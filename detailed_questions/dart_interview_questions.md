# Detailed Guides: Dart Questions

[← Back to Dart Index](../dart_interview_questions.md)

---

## Easy Questions

### Easy 1. What is Dart and what are its key features?

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

Dart is a client-optimized, object-oriented programming language developed by Google. It is used to build fast apps for mobile, web, and desktop. Key features include:
- **Sound Type System:** Safe and predictable code with null safety.
- **JIT & AOT Compilation:** JIT (Just-In-Time) compilation enables fast development and Hot Reload, while AOT (Ahead-Of-Time) compiles code to native machine instructions for production performance.
- **Single Threaded with Event Loop:** Handles asynchronous operations smoothly using an event loop.

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/dart_interview_questions_sort.md#easy-1-what-is-dart-and-what-are-its-key-features)

---

### Easy 2. What are the basic data types in Dart?

**Category:** Data Types &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

Dart supports the following core data types:
- **`int`:** Integer numbers (e.g., `1`, `42`).
- **`double`:** Floating-point numbers (e.g., `3.14`, `0.5`).
- **`num`:** The parent class of both `int` and `double`.
- **`String`:** UTF-16 text representation (e.g., `'Hello Dart'`).
- **`bool`:** Boolean values (`true` and `false`).
- **`List`:** Ordered collections (arrays).
- **`Set`:** Unordered collections of unique values.
- **`Map`:** Key-value pairs.

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/dart_interview_questions_sort.md#easy-2-what-are-the-basic-data-types-in-dart)

---

### Easy 3. What is the difference between var, final, and const?

**Category:** Variables &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

- **`var`:** Declares a mutable variable whose type is automatically inferred by the compiler during its first assignment.
- **`final`:** Declares a read-only variable that can only be set once. Its value is determined at runtime.
- **`const`:** Declares a compile-time constant. Its value must be known and set before compilation, and it is implicitly final.

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/dart_interview_questions_sort.md#easy-3-what-is-the-difference-between-var-final-and-const)

---

### Easy 4. What are optional parameters in Dart (named vs positional)?

**Category:** Functions &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

Optional parameters allow functions to be called without passing all arguments:
- **Named Optional Parameters:** Enclosed in curly braces `{}`. They are passed by name and can be in any order. Can be marked as `required`.
  ```dart
  void greet({String name = 'Guest'}) {}
  ```
- **Positional Optional Parameters:** Enclosed in square brackets `[]`. They must be passed in the exact order they are declared.
  ```dart
  void greet([String name = 'Guest']) {}
  ```

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/dart_interview_questions_sort.md#easy-4-what-are-optional-parameters-in-dart-named-vs-positional)

---

### Easy 5. What is the purpose of the main() function in Dart?

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

The `main()` function is the mandatory entry point of every Dart program. When the program runs, execution starts here. It has a `void` return type and can optionally accept arguments from the command line using `List<String> args`.

```dart
void main() {
  print('Hello, Dart!');
}
```

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/dart_interview_questions_sort.md#easy-5-what-is-the-purpose-of-the-main-function-in-dart)

---

### Easy 6. Explain string interpolation in Dart.

**Category:** Data Types &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

String interpolation allows you to embed variables or expressions directly inside a string literal using the `$` symbol. For complex expressions, wrap them in curly braces `${}`:

```dart
String name = 'Dart';
print('Hello $name'); // Hello Dart

int age = 10;
print('Next year: ${age + 1}'); // Next year: 11
```

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/dart_interview_questions_sort.md#easy-6-explain-string-interpolation-in-dart)

---

### Easy 7. What are null-aware operators in Dart (??, ?., ??=)?

**Category:** Operators &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

Null-aware operators safely handle `null` variables:
- **`??` (If-Null):** Evaluates the left side; if null, it returns the right side.
- **`?.` (Conditional Access):** Accesses a property/method only if the object is not null.
- **`??=` (Null-Aware Assignment):** Assigns a value to a variable only if the variable is currently null.

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/dart_interview_questions_sort.md#easy-7-what-are-null-aware-operators-in-dart)

---

### Easy 8. What is the difference between division (/) and integer division (~/) operators?

**Category:** Operators &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

- **`/` (Standard Division):** Performs division and always returns a floating-point number (`double`), even if the division is clean.
  ```dart
  print(5 / 2); // 2.5
  ```
- **`~/` (Integer Division):** Performs division and discards the decimal remainder, returning only the whole integer quotient (`int`).
  ```dart
  print(5 ~/ 2); // 2
  ```

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/dart_interview_questions_sort.md#easy-8-what-is-the-difference-between-division-and-integer-division-operators)

---

### Easy 9. What are collections in Dart (List, Set, Map)?

**Category:** Collections &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

- **`List`:** An ordered collection of items that allows duplicate values.
- **`Set`:** An unordered collection of unique items; duplicates are automatically ignored.
- **`Map`:** A collection of key-value pairs where keys must be unique and map to values.

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/dart_interview_questions_sort.md#easy-9-what-are-collections-in-dart-list-set-map)

---

### Easy 10. What is the difference between double-quoted and single-quoted string literals in Dart?

**Category:** Data Types &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

There is no functional difference between single quotes (`'...'`) and double quotes (`"..."`) in Dart. The style guide recommends using single quotes for consistency. However, double quotes are useful when a string contains a single quote contraction to avoid escaping characters:

```dart
String s1 = 'It\'s Dart';
String s2 = "It's Dart"; // No escaping needed
```

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/dart_interview_questions_sort.md#easy-10-what-is-the-difference-between-double-quoted-and-single-quoted-string-literals-in-dart)

---

---

### Easy 11. What is the cascade operator (..) in Dart and how does it help write cleaner code?

The cascade operator (`..` and `?..`) allows you to make a sequence of operations on the same object. This saves you from creating temporary variables or repeating the object's name across multiple lines.

#### Example without Cascade
```dart
var paint = Paint();
paint.color = Colors.black;
paint.strokeCap = StrokeCap.round;
paint.strokeWidth = 5.0;
```

#### Example with Cascade
```dart
var paint = Paint()
  ..color = Colors.black
  ..strokeCap = StrokeCap.round
  ..strokeWidth = 5.0;
```

If the object can be null, use the null-aware cascade operator (`?..`):
```dart
paint?..color = Colors.red
     ..strokeWidth = 2.0;
```

[Back to Index](../dart_interview_questions.md#easy-questions) | [Quick Revision](../sort_questions/dart_interview_questions_sort.md#easy-11-what-is-the-cascade-operator-in-dart-and-how-does-it-help-write-cleaner-code)

---

### Easy 12. Explain the spread operator (...) and null-aware spread operator (...?) in Dart collections.

The spread operator (`...`) provides a clean way to insert multiple elements from one collection into another collection.

#### Examples
```dart
var list1 = [1, 2, 3];
var list2 = [0, ...list1, 4]; // Result: [0, 1, 2, 3, 4]
```

If the collection being spread might be null, using `...` will throw a runtime exception. To prevent this, use the null-aware spread operator (`...?`):
```dart
List<int>? list1;
var list2 = [0, ...?list1, 4]; // Result: [0, 4] (no exception thrown)
```

[Back to Index](../dart_interview_questions.md#easy-questions) | [Quick Revision](../sort_questions/dart_interview_questions_sort.md#easy-12-explain-the-spread-operator-and-null-aware-spread-operator-in-dart-collections)

## Medium Questions

### Medium 1. What are Dart Mixins and how do you use them?

**Category:** OOP &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

Mixins are classes containing methods and properties that can be shared and reused by other classes without using class inheritance. A class uses a mixin via the `with` keyword. Mixins are declared using the `mixin` keyword:

```dart
mixin Walker {
  void walk() => print('Walking...');
}

class Dog extends Animal with Walker {}
```

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/dart_interview_questions_sort.md#medium-1-what-are-dart-mixins-and-how-do-you-use-them)

---

### Medium 2. What is the difference between implements, extends, and with?

**Category:** OOP &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

- **`extends`:** Subclasses a single parent class (inheritance). You inherit methods and variables and can override them.
- **`implements`:** Conforms to an interface. You must override and provide implementations for every method and property of the class.
- **`with`:** Applies mixin classes, importing their implementations directly without subclassing.

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/dart_interview_questions_sort.md#medium-2-what-is-the-difference-between-implements-extends-and-with)

---

### Medium 3. What is a factory constructor in Dart and when should you use it?

**Category:** OOP &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

A `factory` constructor is a constructor that does not always create a new instance of its class. Use cases include:
- **Singletons:** Returning a single cached static instance.
- **Caching:** Fetching instance variables from a cache pool.
- **Subclassing:** Returning an instance of a child class depending on parameters.

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/dart_interview_questions_sort.md#medium-3-what-is-a-factory-constructor-in-dart-and-when-should-you-use-it)

---

### Medium 4. Explain the difference between Future and Stream.

**Category:** Asynchrony &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

- **`Future`:** Represents a single asynchronous calculation that will complete in the future, delivering either a single value or an error once.
- **`Stream`:** Represents an active source of asynchronous data events. It delivers multiple data elements over a period of time (like button clicks, websocket updates, or clock ticks).

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/dart_interview_questions_sort.md#medium-4-explain-the-difference-between-future-and-stream)

---

### Medium 5. What are extension methods in Dart?

**Category:** OOP &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

Extension methods allow you to add new functions and getters to existing classes and libraries (even core types like `String` or `int`) without modifying their source code or using subclassing:

```dart
extension Capitalize on String {
  String get upperFirst => this[0].toUpperCase() + substring(1);
}

// Usage
print('hello'.upperFirst); // Hello
```

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/dart_interview_questions_sort.md#medium-5-what-are-extension-methods-in-dart)

---

### Medium 6. What is the difference between dynamic and Object?

**Category:** Type System &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

- **`Object`:** The parent root class of all non-nullable types in Dart. Variables declared as `Object` maintain compile-time type safety; you can only call methods defined on `Object` unless you explicitly check and cast the type.
- **`dynamic`:** A keyword that disables static type checking. You can call any method or property on a dynamic variable. Mismatches will only throw errors at runtime.

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/dart_interview_questions_sort.md#medium-6-what-is-the-difference-between-dynamic-and-object)

---

### Medium 7. Explain late variables (late keyword) and their use cases in null safety.

**Category:** Variables &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

The `late` keyword has two main purposes under null safety:
1. **Deferred Initialization:** Declares a non-nullable variable that will be initialized *after* its declaration (before it is read), satisfying the compiler.
2. **Lazy Loading:** Postpones expensive calculations. The variable is only initialized when it is first accessed, not when the class is constructed.

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/dart_interview_questions_sort.md#medium-7-explain-late-variables-late-keyword-and-their-use-cases-in-null-safety)

---

### Medium 8. What is a typedef in Dart?

**Category:** Type System &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

A `typedef` (type alias) is a way to define a custom, readable name for complex types, most commonly function signatures or generic collections. It makes code cleaner and easier to write:

```dart
typedef OnClick = void Function(int id);

// Usage
final OnClick clickCallback;
```

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/dart_interview_questions_sort.md#medium-8-what-is-a-typedef-in-dart)

---

### Medium 9. What is a Callable class in Dart?

**Category:** OOP &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

A callable class is a Dart class that can be called like a function. To make a class callable, you implement a method named exactly `call()` with any return type and parameter list:

```dart
class Adder {
  int call(int a, int b) => a + b;
}

// Usage
var adder = Adder();
print(adder(2, 3)); // 5
```

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/dart_interview_questions_sort.md#medium-9-what-is-a-callable-class-in-dart)

---

### Medium 10. How do you handle exceptions in Dart (try, catch, finally, throw)?

**Category:** Exception Handling &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

Exceptions are handled using structured blocks:
- **`throw`:** Triggers an error/exception.
- **`try`:** Encloses code that might throw.
- **`on`:** Catches specific exception types.
- **`catch`:** Accesses the exception object (`e`) and stack trace (`s`).
- **`finally`:** Code block that executes regardless of whether an exception occurred, used for cleanup.

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/dart_interview_questions_sort.md#medium-10-how-do-you-handle-exceptions-in-dart-try-catch-finally-throw)

---

### Medium 11. What is the difference between async/await and .then() callbacks?

**Category:** Asynchrony &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

- **`async/await`:** A modern syntax that pauses code execution inside a method until the Future completes. It makes asynchronous code look synchronous and easy to read.
- **`.then()`:** Registers callbacks. The program registers the callback and immediately continues to execute the next lines, making nested futures hard to read (callback hell).

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/dart_interview_questions_sort.md#medium-11-what-is-the-difference-between-asyncawait-and-then-callbacks)

---

### Medium 12. What are Records in Dart 3 and how are they useful?

**Category:** Dart 3 &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

Records are anonymous, immutable, aggregate types introduced in Dart 3. They allow you to bundle multiple values together into a single object without defining a custom class. They are highly useful for returning multiple values from a function:

```dart
(int, String) getUser() {
  return (1, 'Alice');
}

// Usage
var user = getUser();
print(user.$1); // 1
```

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/dart_interview_questions_sort.md#medium-12-what-are-records-in-dart-3-and-how-are-they-useful)

---

---

### Medium 13. What are class modifiers in Dart 3 (such as base, interface, final, sealed) and how do they control inheritance?

Dart 3 introduced class modifiers to give developers control over how classes can be inherited, implemented, or instantiated outside their declaring library.

#### Modifiers
- **`base`**: Allows subclasses to extend (`extends`) the class but blocks them from implementing (`implements`) its interface.
- **`interface`**: Allows other classes to implement (`implements`) the class's interface but blocks extension (`extends`).
- **`final`**: Blocks both inheritance and implementation outside of the library. It can only be instantiated.
- **`sealed`**: Blocks external inheritance, implementation, and instantiation. Subclasses must be defined in the same file, allowing the compiler to perform exhaustiveness checks in switch statements.

[Back to Index](../dart_interview_questions.md#medium-questions) | [Quick Revision](../sort_questions/dart_interview_questions_sort.md#medium-13-what-are-class-modifiers-in-dart-3-and-how-do-they-control-inheritance)

---

### Medium 14. What is the difference between a sealed class and an enum in Dart?

While both `sealed` classes and `enum` types restrict the possible subtypes or values to a fixed set, they have different use cases:

#### Comparison
- **`enum`**: Represents a fixed set of constant *values*. Every value is identical in structure and does not contain unique state instances (e.g., `enum Status { loading, success, error }`).
- **`sealed` class**: Represents a fixed set of *types* (subclasses). Each subclass can be instantiated with its own unique properties, parameters, and behaviors (e.g., `class Success extends Status { final String data; ... }`).

#### Common Use Case
Sealed classes are widely used in state management to represent distinct UI states where different states hold different types of payload data (e.g., an `Error` state holding a message string, and `Loaded` holding a query result).

[Back to Index](../dart_interview_questions.md#medium-questions) | [Quick Revision](../sort_questions/dart_interview_questions_sort.md#medium-14-what-is-the-difference-between-a-sealed-class-and-an-enum-in-dart)

---

### Medium 15. What is a StreamController and how does a single-subscription stream differ from a broadcast stream?

A `StreamController` is used to create and manage streams in Dart. It provides a `sink` to add data/events and a `stream` to listen to them.

#### Stream Types
1. **Single-Subscription Stream**:
   - Allows only one listener during its entire lifetime.
   - If you try to listen to it a second time, it throws an exception.
   - It is designed for sequential data (e.g., file downloads).
2. **Broadcast Stream**:
   - Allows multiple listeners to subscribe simultaneously.
   - Events are sent to all active listeners.
   - Listeners only receive events sent after they subscribe.
   - It is designed for independent, real-time events (e.g., UI clicks, sensor events).

```dart
// Creating a broadcast stream controller
final controller = StreamController<int>.broadcast();
```

[Back to Index](../dart_interview_questions.md#medium-questions) | [Quick Revision](../sort_questions/dart_interview_questions_sort.md#medium-15-what-is-a-streamcontroller-and-how-does-a-single-subscription-stream-differ-from-a-broadcast-stream)

## Hard Questions

### Hard 1. How does the Dart Event Loop work? (Microtask vs Event Queue)

**Category:** Asynchrony &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Hard

Dart is single-threaded. Its event loop processes tasks from two queues in order:
1. **Microtask Queue:** Holds short, internal framework tasks. It takes priority. The loop processes microtasks until this queue is completely empty.
2. **Event Queue:** Holds external events (I/O, clicks, drawing, timers). The loop processes one event, then immediately checks and clears the microtask queue before processing the next event.
This ensures system-level updates execute immediately.

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/dart_interview_questions_sort.md#hard-1-how-does-the-dart-event-loop-work-microtask-vs-event-queue)

---

### Hard 2. What is an Isolate in Dart, and how do you communicate between them?

**Category:** Concurrency &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Hard

An Isolate is Dart's concurrency model. Unlike traditional threads, isolates do not share memory; each has its own private memory heap and event loop. This prevents race conditions and locks. Isolates can only communicate by sending messages asynchronously over ports using a `SendPort` and a `ReceivePort` setup.

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/dart_interview_questions_sort.md#hard-2-what-is-an-isolate-in-dart-and-how-do-you-communicate-between-them)

---

### Hard 3. What are Generators in Dart (sync* / yield and async* / yield*)?

**Category:** Asynchrony &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Hard

Generators lazily produce values on demand:
- **Synchronous Generator (`sync*`):** Returns an `Iterable`. It uses `yield` to return a value, pausing execution until the iterator requests the next value.
- **Asynchronous Generator (`async*`):** Returns a `Stream`. It uses `yield` to push values to the stream asynchronously.
- **`yield*`:** Delegate production to another nested generator/collection.

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/dart_interview_questions_sort.md#hard-3-what-are-generators-in-dart-sync-yield-and-async-yield)

---

### Hard 4. How does garbage collection work in Dart?

**Category:** Architecture &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Hard

Dart uses a two-generational garbage collector (GC) optimized for client UIs:
1. **Young Generation (Scavenger):** Fast, copy-based collector. It processes short-lived objects (like widgets created during frame rebuilding) by copying active objects to a new space and freeing the old one.
2. **Old Generation (Mark-Sweep-Compact):** Handles long-lived objects. It sweeps through the memory heap, marks active objects, deletes unreferenced ones, and defragments (compacts) memory space.

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/dart_interview_questions_sort.md#hard-4-how-does-garbage-collection-work-in-dart)

---

### Hard 5. Explain soundness in Dart's type system (type safety, covariance).

**Category:** Type System &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Hard

Soundness guarantees that a variable's runtime value matches its compile-time static type, ensuring that type errors never occur at runtime. Dart supports **covariance**, which allows a subtype to be used where a supertype is expected (e.g., passing a `List<Cat>` to a function expecting `List<Animal>`). Soundness catches type violations statically.

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/dart_interview_questions_sort.md#hard-5-explain-soundness-in-darts-type-system-type-safety-covariance)

---

### Hard 6. What is the difference between JIT and AOT compilation in the Dart VM?

**Category:** Architecture &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Hard

- **JIT (Just-in-Time):** Compiles code dynamically during runtime. It enables developer tools like Hot Reload and hot debugging by allowing the Dart VM to reload updated source files instantly.
- **AOT (Ahead-of-Time):** Compiles code directly into native platform machine instructions before deployment. It optimizes app startup speed, reduces size, and runs code at native execution speed.

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/dart_interview_questions_sort.md#hard-6-what-is-the-difference-between-jit-and-aot-compilation-in-the-dart-vm)

---

### Hard 7. What are Extension Types and how do they differ from extension methods or wrapper classes?

**Category:** Dart 3 &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Hard

Introduced in Dart 3.3, an **Extension Type** provides a compile-time-only wrapper around an existing type. Unlike wrapper classes, extension types have zero runtime overhead because they compile directly to the underlying representation. They differ from extension methods by defining a completely new type interface rather than just adding utility methods to an existing type:

```dart
extension type Id(int value) {}
// At runtime, 'Id' is just a raw integer with no wrapper class wrapper!
```

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/dart_interview_questions_sort.md#hard-7-what-are-extension-types-and-how-do-they-differ-from-extension-methods-or-wrapper-classes)

---

### Hard 8. How do you implement custom StreamTransformers in Dart?

**Category:** Streams &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Hard

To create a custom StreamTransformer, you implement the `StreamTransformer` class and override its `bind()` method. It receives a source stream, applies custom filtering, mapping, or logic, and returns a modified stream. It is typically created using `StreamTransformer.fromHandlers` for simplicity:

```dart
final myTransformer = StreamTransformer<int, String>.fromHandlers(
  handleData: (data, sink) => sink.add('Value: $data'),
);
```

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/dart_interview_questions_sort.md#hard-8-how-do-you-implement-custom-streamtransformers-in-dart)

---

### Hard 9. What is Zone in Dart, and what is it used for?

**Category:** Architecture &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Hard

A `Zone` is an execution context that persists across asynchronous operations. It is used to:
- **Catch Unhandled Errors:** Intercept all asynchronous errors globally using a custom error zone (`runZonedGuarded`).
- **Track Operations:** Track or time asynchronous executions.
- **Override Core Behaviors:** Override printing, zones, or microtask scheduling globally (e.g., for unit testing mocks).

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/dart_interview_questions_sort.md#hard-9-what-is-zone-in-dart-and-what-is-it-used-for)

---

### Hard 10. How does Dart handle memory management and avoid memory leaks with streams?

**Category:** Architecture &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Hard

Streams can cause memory leaks if subscriptions are left open when a widget is destroyed. To prevent leaks:
1. **Cancel Subscriptions:** Call `.cancel()` on `StreamSubscription` in the widget's `dispose()` lifecycle method.
2. **Close Controllers:** Call `.close()` on `StreamController` objects.
3. **Use StreamBuilder:** Use the `StreamBuilder` widget, which automatically handles subscription and cleanup logic internally.

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/dart_interview_questions_sort.md#hard-10-how-does-dart-handle-memory-management-and-avoid-memory-leaks-with-streams)

---

### Hard 11. Explain pattern matching and destructuring in Dart 3.

**Category:** Dart 3 &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Hard

Dart 3 introduced pattern matching and destructuring, which allows you to inspect structure, extract values, and match patterns directly inside assignments, control structures, and switch statements:

```dart
// Destructuring a record
var (name, age) = ('Bob', 30);

// Pattern matching in a switch
switch (pair) {
  case (0, var y): print('X is zero, Y is $y');
  default: print('No match');
}
```

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/dart_interview_questions_sort.md#hard-11-explain-pattern-matching-and-destructuring-in-dart-3)

---

---

### Hard 12. Explain variance and the covariant keyword in Dart's type system.

Variance describes how type relationships of generic parameters affect the subtype relationships of the classes containing them.

#### Covariance in generics
In Dart, generic parameters on classes are **covariant** by default. This means if `Dog` is a subclass of `Animal`, then `List<Dog>` is treated as a subclass of `List<Animal>`. While safe for reading data, covariance can cause runtime type exceptions when writing data.

#### The `covariant` Keyword
The `covariant` keyword tells the compiler to allow a method parameter in a subclass to be a more specific subtype than what is declared in the parent class.

```dart
abstract class AnimalFeed {}
class DogFood extends AnimalFeed {}

class Animal {
  void eat(AnimalFeed feed) {}
}

class Dog extends Animal {
  @override
  // Without 'covariant', this override would cause a static analysis error
  void eat(covariant DogFood feed) {}
}
```

[Back to Index](../dart_interview_questions.md#hard-questions) | [Quick Revision](../sort_questions/dart_interview_questions_sort.md#hard-12-explain-variance-and-the-covariant-keyword-in-darts-type-system)

---

### Hard 13. What are Dart Macros (Metaprogramming) and how do they change static code generation in Dart?

Dart Macros represent a compile-time metaprogramming feature designed to replace static code generation tools like `build_runner` (used for `freezed`, `json_serializable`, etc.).

#### How it works
Macros compile and execute *during the static analysis/compilation phase* of Dart. They inspect the existing code structure (such as class fields or methods) and generate additional Dart code directly into the compiler's memory tree.

#### Key Benefits
- **No File Clutter**: No need to generate `.g.dart` or `.freezed.dart` files.
- **Instant Updates**: Code is generated in real-time as you type, rather than waiting for long `dart run build_runner build` runs.
- **IDE Integration**: The IDE can see and navigate to the macro-generated members immediately.

[Back to Index](../dart_interview_questions.md#hard-questions) | [Quick Revision](../sort_questions/dart_interview_questions_sort.md#hard-13-what-are-dart-macros-metaprogramming-and-how-do-they-change-static-code-generation-in-dart)

