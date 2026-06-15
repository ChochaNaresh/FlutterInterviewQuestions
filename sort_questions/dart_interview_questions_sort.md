# Quick Revision: Dart Questions

Condensed 1-4 sentence answers for last-minute review.

[← Back to Dart Index](../dart_interview_questions.md)

---

## Easy Questions

### Easy 1. What is Dart and what are its key features?

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

*Dart is Google's client-optimized, object-oriented language. Key features include a sound type system, JIT/AOT compilation, and event-loop driven asynchronous support.*

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Detailed Guide](../detailed_questions/dart_interview_questions.md#easy-1-what-is-dart-and-what-are-its-key-features)

---

### Easy 2. What are the basic data types in Dart?

**Category:** Data Types &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

*Dart's basic data types are `int`, `double` (and their parent `num`), `String`, `bool`, along with collections like `List`, `Set`, and `Map`.*

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Detailed Guide](../detailed_questions/dart_interview_questions.md#easy-2-what-are-the-basic-data-types-in-dart)

---

### Easy 3. What is the difference between var, final, and const?

**Category:** Variables &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

*`var` is mutable, `final` is runtime-constant, and `const` is a compile-time constant.*

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Detailed Guide](../detailed_questions/dart_interview_questions.md#easy-3-what-is-the-difference-between-var-final-and-const)

---

### Easy 4. What are optional parameters in Dart (named vs positional)?

**Category:** Functions &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

*Named parameters (defined in `{}`) are referenced by name, whereas positional optional parameters (defined in `[]`) are passed by order.*

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Detailed Guide](../detailed_questions/dart_interview_questions.md#easy-4-what-are-optional-parameters-in-dart-named-vs-positional)

---

### Easy 5. What is the purpose of the main() function in Dart?

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

*The `main()` function is the execution entry point for every Dart application.*

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Detailed Guide](../detailed_questions/dart_interview_questions.md#easy-5-what-is-the-purpose-of-the-main-function-in-dart)

---

### Easy 6. Explain string interpolation in Dart.

**Category:** Data Types &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

*String interpolation embeds variables (`$variable`) or expressions (`${expression}`) directly within string literals.*

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Detailed Guide](../detailed_questions/dart_interview_questions.md#easy-6-explain-string-interpolation-in-dart)

---

### Easy 7. What are null-aware operators in Dart (??, ?., ??=)?

**Category:** Operators &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

*Null-aware operators (`??`, `?.`, `??=`) allow you to access properties and assign fallback values safely for variables that might be null.*

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Detailed Guide](../detailed_questions/dart_interview_questions.md#easy-7-what-are-null-aware-operators-in-dart)

---

### Easy 8. What is the difference between division (/) and integer division (~/) operators?

**Category:** Operators &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

*The `/` operator returns a double with decimals, whereas the `~/` operator returns only the whole integer portion.*

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Detailed Guide](../detailed_questions/dart_interview_questions.md#easy-8-what-is-the-difference-between-division-and-integer-division-operators)

---

### Easy 9. What are collections in Dart (List, Set, Map)?

**Category:** Collections &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

*Lists are ordered with duplicates allowed, Sets are unordered with unique values, and Maps store key-value associations.*

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Detailed Guide](../detailed_questions/dart_interview_questions.md#easy-9-what-are-collections-in-dart-list-set-map)

---

### Easy 10. What is the difference between double-quoted and single-quoted string literals in Dart?

**Category:** Data Types &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

*Single and double quotes are functionally identical, but single quotes are preferred. Double quotes are useful to avoid escaping single quote apostrophes.*

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Detailed Guide](../detailed_questions/dart_interview_questions.md#easy-10-what-is-the-difference-between-double-quoted-and-single-quoted-string-literals-in-dart)

---


## Medium Questions

### Medium 1. What are Dart Mixins and how do you use them?

**Category:** OOP &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

*Mixins enable sharing code across multiple classes without subclassing. They are declared using the `mixin` keyword and applied with `with`.*

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Detailed Guide](../detailed_questions/dart_interview_questions.md#medium-1-what-are-dart-mixins-and-how-do-you-use-them)

---

### Medium 2. What is the difference between implements, extends, and with?

**Category:** OOP &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

*`extends` inherits from a single class, `implements` forces code to define all interface members, and `with` applies reusable mixin code.*

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Detailed Guide](../detailed_questions/dart_interview_questions.md#medium-2-what-is-the-difference-between-implements-extends-and-with)

---

### Medium 3. What is a factory constructor in Dart and when should you use it?

**Category:** OOP &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

*A factory constructor is used when you want a constructor to return cached, existing instances (Singleton) or subclasses instead of a new object.*

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Detailed Guide](../detailed_questions/dart_interview_questions.md#medium-3-what-is-a-factory-constructor-in-dart-and-when-should-you-use-it)

---

### Medium 4. Explain the difference between Future and Stream.

**Category:** Asynchrony &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

*A `Future` yields a single asynchronous result once, while a `Stream` delivers multiple asynchronous data events over time.*

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Detailed Guide](../detailed_questions/dart_interview_questions.md#medium-4-explain-the-difference-between-future-and-stream)

---

### Medium 5. What are extension methods in Dart?

**Category:** OOP &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

*Extension methods let you add custom functionality to existing classes without editing their code or subclassing them.*

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Detailed Guide](../detailed_questions/dart_interview_questions.md#medium-5-what-are-extension-methods-in-dart)

---

### Medium 6. What is the difference between dynamic and Object?

**Category:** Type System &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

*`Object` is type-safe and requires casting to call subclass methods, while `dynamic` disables compile-time checks, risking runtime errors.*

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Detailed Guide](../detailed_questions/dart_interview_questions.md#medium-6-what-is-the-difference-between-dynamic-and-object)

---

### Medium 7. Explain late variables (late keyword) and their use cases in null safety.

**Category:** Variables &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

*The `late` keyword is used for declaring non-nullable variables that will be initialized later, and for lazy-loading expensive calculations.*

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Detailed Guide](../detailed_questions/dart_interview_questions.md#medium-7-explain-late-variables-late-keyword-and-their-use-cases-in-null-safety)

---

### Medium 8. What is a typedef in Dart?

**Category:** Type System &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

*A `typedef` creates a custom alias for a complex type signature, making function parameter typing cleaner and more reusable.*

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Detailed Guide](../detailed_questions/dart_interview_questions.md#medium-8-what-is-a-typedef-in-dart)

---

### Medium 9. What is a Callable class in Dart?

**Category:** OOP &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

*A callable class implements the `call()` method, enabling class instances to be invoked directly like normal functions.*

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Detailed Guide](../detailed_questions/dart_interview_questions.md#medium-9-what-is-a-callable-class-in-dart)

---

### Medium 10. How do you handle exceptions in Dart (try, catch, finally, throw)?

**Category:** Exception Handling &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

*Exceptions are thrown using `throw`, caught using `try-catch` (with optional `on` for type filtering), and cleaned up inside `finally` blocks.*

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Detailed Guide](../detailed_questions/dart_interview_questions.md#medium-10-how-do-you-handle-exceptions-in-dart-try-catch-finally-throw)

---

### Medium 11. What is the difference between async/await and .then() callbacks?

**Category:** Asynchrony &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

*`async/await` makes asynchronous code sequential and easy to read, whereas `.then()` uses callbacks which can lead to nested code blocks.*

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Detailed Guide](../detailed_questions/dart_interview_questions.md#medium-11-what-is-the-difference-between-asyncawait-and-then-callbacks)

---

### Medium 12. What are Records in Dart 3 and how are they useful?

**Category:** Dart 3 &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

*Records are anonymous, immutable groupings of values that let functions return multiple values cleanly without custom classes.*

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Detailed Guide](../detailed_questions/dart_interview_questions.md#medium-12-what-are-records-in-dart-3-and-how-are-they-useful)

---


## Hard Questions

### Hard 1. How does the Dart Event Loop work? (Microtask vs Event Queue)

**Category:** Asynchrony &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Hard

*The event loop runs microtasks first, then processes event queue items one by one, checking for new microtasks between every event.*

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Detailed Guide](../detailed_questions/dart_interview_questions.md#hard-1-how-does-the-dart-event-loop-work-microtask-vs-event-queue)

---

### Hard 2. What is an Isolate in Dart, and how do you communicate between them?

**Category:** Concurrency &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Hard

*Isolates are independent threads that do not share memory. They communicate solely through message passing via ports.*

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Detailed Guide](../detailed_questions/dart_interview_questions.md#hard-2-what-is-an-isolate-in-dart-and-how-do-you-communicate-between-them)

---

### Hard 3. What are Generators in Dart (sync* / yield and async* / yield*)?

**Category:** Asynchrony &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Hard

*Generators produce sequences lazily: `sync*` returns an `Iterable` using synchronous yields, and `async*` returns a `Stream` using async yields.*

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Detailed Guide](../detailed_questions/dart_interview_questions.md#hard-3-what-are-generators-in-dart-sync-yield-and-async-yield)

---

### Hard 4. How does garbage collection work in Dart?

**Category:** Architecture &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Hard

*Dart uses a generational GC: a fast scavenger for short-lived widgets, and a mark-sweep-compact collector for long-lived objects.*

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Detailed Guide](../detailed_questions/dart_interview_questions.md#hard-4-how-does-garbage-collection-work-in-dart)

---

### Hard 5. Explain soundness in Dart's type system (type safety, covariance).

**Category:** Type System &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Hard

*Soundness ensures static types match runtime values, preventing type errors. Covariance allows substituting subtypes for supertypes safely.*

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Detailed Guide](../detailed_questions/dart_interview_questions.md#hard-5-explain-soundness-in-darts-type-system-type-safety-covariance)

---

### Hard 6. What is the difference between JIT and AOT compilation in the Dart VM?

**Category:** Architecture &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Hard

*JIT compiles code dynamically at runtime for fast development, while AOT pre-compiles code to native binary for fast release execution.*

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Detailed Guide](../detailed_questions/dart_interview_questions.md#hard-6-what-is-the-difference-between-jit-and-aot-compilation-in-the-dart-vm)

---

### Hard 7. What are Extension Types and how do they differ from extension methods or wrapper classes?

**Category:** Dart 3 &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Hard

*Extension Types are compile-time-only wrapper interfaces with zero runtime overhead, compiling directly to their underlying raw type.*

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Detailed Guide](../detailed_questions/dart_interview_questions.md#hard-7-what-are-extension-types-and-how-do-they-differ-from-extension-methods-or-wrapper-classes)

---

### Hard 8. How do you implement custom StreamTransformers in Dart?

**Category:** Streams &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Hard

*Custom StreamTransformers filter or modify stream events by implementing `StreamTransformer` and overriding the `bind` method.*

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Detailed Guide](../detailed_questions/dart_interview_questions.md#hard-8-how-do-you-implement-custom-streamtransformers-in-dart)

---

### Hard 9. What is Zone in Dart, and what is it used for?

**Category:** Architecture &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Hard

*A Zone is an asynchronous execution context used to catch global async errors, track executions, and override system operations.*

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Detailed Guide](../detailed_questions/dart_interview_questions.md#hard-9-what-is-zone-in-dart-and-what-is-it-used-for)

---

### Hard 10. How does Dart handle memory management and avoid memory leaks with streams?

**Category:** Architecture &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Hard

*To prevent stream memory leaks, always cancel subscriptions and close stream controllers in `dispose()`, or use `StreamBuilder`.*

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Detailed Guide](../detailed_questions/dart_interview_questions.md#hard-10-how-does-dart-handle-memory-management-and-avoid-memory-leaks-with-streams)

---

### Hard 11. Explain pattern matching and destructuring in Dart 3.

**Category:** Dart 3 &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Hard

*Pattern matching in Dart 3 lets you check properties and destructure complex data values (like records) directly inside statements.*

[Back to Index](../dart_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Detailed Guide](../detailed_questions/dart_interview_questions.md#hard-11-explain-pattern-matching-and-destructuring-in-dart-3)

---
