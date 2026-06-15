# Builder & Code Generation Interview Questions - Detailed Explanations

This guide contains detailed answers, code examples, and trade-offs for 10 Builder & Code Generation interview questions.

## Easy Questions

### Easy 1. What is code generation (codegen) in Flutter and why is it useful?

Code generation is the automated process of creating valid Dart source files using automated scripts (`build_runner`) based on class annotations.

#### Why it is useful
- **Eliminates Boilerplate**: Automates repetitive code like writing serialized `fromJson` mappings, equality operators, hashcodes, or immutable copy structures.
- **Reduces Human Error**: Hand-written parsing code is error-prone. Generated code is guaranteed to be syntactically correct and consistent.
- **Improves Maintenance**: If class properties are renamed or added, you simply regenerate the code instead of manually modifying multiple mapping functions.

[Back to Index](../builder_interview_questions.md#easy-questions) | [Quick Revision](../sort_questions/builder_interview_questions_sort.md#easy-1-what-is-code-generation-codegen-in-flutter-and-why-is-it-useful)

### Easy 2. What is the purpose of the freezed package?

`freezed` is a code generator used to create immutable data classes and union/sealed classes in Dart.

#### What it provides out of the box
- **Immutability**: All fields are final, forcing objects to be modified through a safe cloning helper (`copyWith`).
- **Value-based Equality**: Overrides `==` and `hashCode` so that two different objects with the exact same data values are evaluated as equal.
- **Union Classes**: Makes it simple to represent distinct class states (like `State.loading()`, `State.success(data)`) for pattern matching.

```dart
@freezed
class User with _$User {
  const factory User({required String name, required int age}) = _User;
}
```

[Back to Index](../builder_interview_questions.md#easy-questions) | [Quick Revision](../sort_questions/builder_interview_questions_sort.md#easy-2-what-is-the-purpose-of-the-freezed-package)

### Easy 3. What is the purpose of the json_serializable package?

`json_serializable` automatically generates the serialization and deserialization code to convert Dart objects to and from JSON maps (`Map<String, dynamic>`).

#### How to use it
- You annotate your Dart model class with `@JsonSerializable()`.
- The package generates a helper file (ending in `.g.dart`) containing serialization code.
- You reference the generated code in your class constructor factories:

```dart
@JsonSerializable()
class User {
  final String name;
  User(this.name);

  factory User.fromJson(Map<String, dynamic> json) => _$UserFromJson(json);
  Map<String, dynamic> toJson() => _$UserToJson(this);
}
```

[Back to Index](../builder_interview_questions.md#easy-questions) | [Quick Revision](../sort_questions/builder_interview_questions_sort.md#easy-3-what-is-the-purpose-of-the-json_serializable-package)

## Medium Questions

### Medium 1. How do you run the code generator and what is the difference between build and watch commands?

To execute builders in Flutter (such as `freezed` or `json_serializable`), you use the `build_runner` CLI tool.

#### The Commands
1. **`dart run build_runner build`**:
   - Runs a single pass over your codebase.
   - It reads your files, finds annotations, generates the matching `.g.dart` or `.freezed.dart` files, and exits.
   - Best for CI/CD pipelines or once-off setups.
2. **`dart run build_runner watch`**:
   - Runs an incremental file watcher process in the background.
   - It watches files for edits and immediately regenerates corresponding files as soon as you save.
   - Best for local development.

*Tip:* Add `--delete-conflicting-outputs` to force overwrite any invalid or outdated generated code files automatically.

[Back to Index](../builder_interview_questions.md#medium-questions) | [Quick Revision](../sort_questions/builder_interview_questions_sort.md#medium-1-how-do-you-run-the-code-generator-and-what-is-the-difference-between-build-and-watch-commands)

### Medium 2. How do you customize json keys (e.g., snake_case to camelCase) using @JsonKey and @JsonSerializable?

Backend responses often use `snake_case`, while Dart variables follow `camelCase`. `json_serializable` provides properties to map these fields automatically.

#### Global Config using `@JsonSerializable`
Instead of mapping variables manually, tell the class serializer to convert all keys to a casing pattern using `fieldRename`:

```dart
@JsonSerializable(fieldRename: FieldRename.snake) // Ex: 'firstName' maps to 'first_name'
class UserProfile {
  final String firstName;
}
```

#### Granular Config using `@JsonKey`
For individual fields that don't match the general rule, override them using `@JsonKey`:

```dart
class UserProfile {
  @JsonKey(name: 'user_auth_token_key')
  final String token;
}
```

[Back to Index](../builder_interview_questions.md#medium-questions) | [Quick Revision](../sort_questions/builder_interview_questions_sort.md#medium-2-how-do-you-customize-json-keys-using-jsonkey-and-jsonserializable)

### Medium 3. What is the copyWith method generated by freezed and why is it important for immutability?

In robust application architectures, state changes should be immutable. Rather than changing properties of an existing object directly, you create a new instance with updated values.

#### The Role of copyWith
The `copyWith` method is an automated utility that clones an object while allowing you to override specific fields.

```dart
// Modifying immutable state
final updatedUser = currentUser.copyWith(age: 26);
```

#### Why it matters
- **Thread Safety:** Prevents unintended bugs where parts of the app modify state behind the scenes.
- **Rebuild Triggers:** Enables frameworks like Riverpod or BLoC to detect changes via object equality checks (`oldState != newState`) to trigger UI updates.

[Back to Index](../builder_interview_questions.md#medium-questions) | [Quick Revision](../sort_questions/builder_interview_questions_sort.md#medium-3-what-is-the-copywith-method-generated-by-freezed-and-why-is-it-important-for-immutability)

### Medium 4. How do you handle default values for properties in a freezed class?

Since `freezed` classes use redirecting factories instead of standard constructor bodies, you cannot assign default parameter values using standard Dart syntax.

#### The Solution
Expose default values using the `@Default()` annotation:

```dart
@freezed
class UserState with _$UserState {
  const factory UserState({
    @Default(true) bool isLoading,
    @Default([]) List<String> items,
  }) = _UserState;
}
```

*Note:* When combining with `json_serializable`, `@Default()` automatically sets fallback values during JSON parsing if keys are missing from the backend response.

[Back to Index](../builder_interview_questions.md#medium-questions) | [Quick Revision](../sort_questions/builder_interview_questions_sort.md#medium-4-how-do-you-handle-default-values-for-properties-in-a-freezed-class)

## Hard Questions

### Hard 1. Explain union/sealed classes in freezed and how they facilitate type-safe state transitions.

`freezed` allows you to define union (or sealed) classes, which represent a fixed closed hierarchy of class variants. This is commonly used to model states in state management architectures.

#### Implementation
```dart
@freezed
class AuthenticationState with _$AuthenticationState {
  const factory AuthenticationState.initial() = _Initial;
  const factory AuthenticationState.loading() = _Loading;
  const factory AuthenticationState.authenticated(User user) = _Authenticated;
  const factory AuthenticationState.error(String message) = _Error;
}
```

#### Why it is powerful
- **Exhaustive pattern matching**: Using `.when` or `.map` methods generated by freezed, the compiler forces you to handle every subclass case. Leaving out the `error` state results in a compilation error.
- **No manual type checks**: Eliminates standard nested `if (state is Loading) {}` blocks, replacing them with a readable, safe switch expression.

[Back to Index](../builder_interview_questions.md#hard-questions) | [Quick Revision](../sort_questions/builder_interview_questions_sort.md#hard-1-explain-unionsealed-classes-in-freezed-and-how-they-facilitate-type-safe-state-transitions)

### Hard 2. How do you implement custom serialization/deserialization for complex types using JsonConverter?

Sometimes, you need to map complex custom types (like `DateTime`, `Color`, or third-party objects) that `json_serializable` cannot serialize automatically.

#### Implementation
1. Create a class extending `JsonConverter<YourType, JSONType>`.
2. Override `fromJson()` and `toJson()` to define custom mapping logic.
3. Annotate your variable with the custom converter class.

```dart
// Custom DateTime converter (e.g. converting timestamp in milliseconds to DateTime)
class EpochDateTimeConverter implements JsonConverter<DateTime, int> {
  const EpochDateTimeConverter();

  @override
  DateTime fromJson(int json) => DateTime.fromMillisecondsSinceEpoch(json);

  @override
  int toJson(DateTime object) => object.millisecondsSinceEpoch;
}

// Applying converter
@JsonSerializable()
class EventLog {
  @EpochDateTimeConverter()
  final DateTime timestamp;
}
```

[Back to Index](../builder_interview_questions.md#hard-questions) | [Quick Revision](../sort_questions/builder_interview_questions_sort.md#hard-2-how-do-you-implement-custom-serializationdeserialization-for-complex-types-using-jsonconverter)

### Hard 3. How does build_runner manage caching, and how do you resolve builder conflicts or build failures?

`build_runner` uses an incremental caching system inside the `.dart_tool/build/` directory to save time on subsequent builds. However, cache states can sometimes get corrupted or run into write conflicts.

#### Resolution Strategies
1. **Overwriting Conflicts**: If output files were modified manually, `build_runner` blocks execution. Resolve this by adding the delete flag:
   ```bash
   dart run build_runner build --delete-conflicting-outputs
   ```
2. **Clearing Cache**: If compile errors persist after refactoring, clean the compiler cache:
   ```bash
   dart run build_runner clean
   # Followed by a fresh build
   dart run build_runner build
   ```
3. **Flutter-Level Clean**: If files are still out of sync, run a root cleanup:
   ```bash
   flutter clean
   flutter pub get
   dart run build_runner build
   ```

[Back to Index](../builder_interview_questions.md#hard-questions) | [Quick Revision](../sort_questions/builder_interview_questions_sort.md#hard-3-how-does-build_runner-manage-caching-and-how-do-you-resolve-builder-conflicts-or-build-failures)
