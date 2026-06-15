# Detailed Guides: Flutter Questions

[← Back to Flutter Index](../flutter_interview_questions.md)

---

## Easy Questions

### Easy 1. What is flutter

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

Flutter is an open-source UI toolkit created by Google. It allows developers to build beautiful, natively compiled applications for mobile (Android & iOS), web, desktop, and embedded devices from a single codebase.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#easy-1-what-is-flutter)

---

### Easy 2. What is dart and why does flutter use it

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

Dart is a client-optimized programming language developed by Google. Flutter uses Dart because:
1. **Declarative Layout:** Dart avoids the need for separate layout languages (like XML or HTML) by defining UI programmatically, making code easy to read.
2. **High Performance:** Dart compiles directly to native machine code (Ahead-of-Time compilation, or AOT), making apps run fast.
3. **Fast Development:** Dart supports Just-in-Time (JIT) compilation, which powers Flutter's Hot Reload feature for instant UI updates.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#easy-2-what-is-dart-and-why-does-flutter-use-it)

---

### Easy 3. What is pubspecyaml file and what does it do

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

The `pubspec.yaml` file is the configuration file for a Flutter project. It is located at the root of the project directory and is used to:
- Define project metadata (name, description, version, and environment constraints).
- Manage external dependencies (packages from pub.dev).
- Declare assets like images, fonts, and configuration files.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#easy-3-what-is-pubspecyaml-file-and-what-does-it-do)

---

### Easy 4. What is the difference between main and runapp functions in flutter

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

In Flutter:
- **`main()`** is the entry point of the Dart program. It tells the Dart runtime where the execution starts.
- **`runApp()`** is a Flutter function that attaches the given root widget to the screen, inflating the widget tree and rendering the user interface.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#easy-4-what-is-the-difference-between-main-and-runapp-functions-in-flutter)

---

### Easy 5. Differentiate between named parameters and positional parameters in flutter

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

- **Positional Parameters:** Parameters that must be passed in the exact order they are declared in the function signature.
- **Named Parameters:** Parameters enclosed in curly braces `{}`. They are passed by specifying the name of the parameter, allowing them to be passed in any order.

```dart
// Positional parameter
void greetPositional(String name, String greeting) {}

// Named parameter
void greetNamed({required String name, String greeting = 'Hello'}) {}
```

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#easy-5-differentiate-between-named-parameters-and-positional-parameters-in-flutter)

---

### Easy 6. What are widgets in flutter

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

In Flutter, a **widget** is an immutable description of a part of the user interface. Everything you see on the screen—including layout elements (padding, columns), styles (themes), and interactive components (buttons, text inputs)—is a widget. Widgets describe how the UI should look given its current configuration and state.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#easy-6-what-are-widgets-in-flutter)

---

### Easy 7. What is hot reload and hot restart in flutter

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

- **Hot Reload:** Inject updated source code files into the running Dart VM. It rebuilds the widget tree while preserving the application state (e.g., inputs, navigation state), allowing you to see changes in seconds.
- **Hot Restart:** Reloads the code changes into the Dart VM and restarts the app from the beginning, losing all saved state.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#easy-7-what-is-hot-reload-and-hot-restart-in-flutter)

---

### Easy 8. What do you mean by open source software is flutter open source

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

Open-source software is software with source code that anyone can inspect, modify, and distribute. Yes, Flutter is open-source. Its source code is hosted on GitHub, allowing the developer community to contribute, inspect, and customize it freely.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#easy-8-what-do-you-mean-by-open-source-software-is-flutter-open-source)

---

### Easy 9. Differentiate between statelesswidget and statefulwidget in flutter

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

- **`StatelessWidget`:** A widget that does not change its state or appearance after it is built. It is immutable and only relies on the configuration data passed to it (e.g., a simple `Text` or `Icon` widget).
- **`StatefulWidget`:** A widget that can dynamically change its appearance or behavior during its lifetime. It has a separate mutable `State` object that stores dynamic data and triggers a rebuild when modified using `setState()` (e.g., `Checkbox` or `TextField`).

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#easy-9-differentiate-between-statelesswidget-and-statefulwidget-in-flutter)

---

### Easy 10. What are packages and plugins in flutter

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

- **Package:** A collection of reusable Dart code. It only contains Dart code and can have dependencies on the Flutter framework (e.g., helper libraries, UI widgets).
- **Plugin:** A special type of package that wraps platform-specific native APIs (Java/Kotlin for Android, Objective-C/Swift for iOS) so they can be called from Dart code using platform channels.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#easy-10-what-are-packages-and-plugins-in-flutter)

---

### Easy 11. Name some popular apps made with flutter

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

Many popular apps are built with Flutter, including:
- **BMW:** Mobile app for vehicle management.
- **Google Pay:** Financial payment app.
- **Alibaba:** Large e-commerce platform.
- **Nubank:** Popular digital banking app.
- **Reflectly:** AI-powered journal app.
- **Hamilton:** Official app for the musical.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#easy-11-name-some-popular-apps-made-with-flutter)

---

### Easy 12. Differentiate between final const and static keyword

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

- **`final`:** A variable whose value can be set only once. It is resolved at runtime.
- **`const`:** A variable whose value must be known and set at compile time. Const values are implicitly final.
- **`static`:** A class-level variable or method that belongs to the class itself rather than instances of the class. It persists state across instances.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#easy-12-differentiate-between-final-const-and-static-keyword)

---

### Easy 13. What is fat arrow notation in dart

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

Fat arrow notation (`=>`) is shorthand syntax in Dart for writing functions that contain a single expression. It automatically returns the value of the expression.

```dart
// Normal syntax
int add(int a, int b) {
  return a + b;
}

// Fat arrow syntax
int add(int a, int b) => a + b;
```

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#easy-13-what-is-fat-arrow-notation-in-dart)

---

### Easy 14. What is the purpose of safearea widget in flutter

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

The `SafeArea` widget wraps a child widget and adds sufficient padding to prevent the operating system from covering it. This avoids intrusions like the camera notch, status bar, navigation bar, and screen corners on modern devices.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#easy-14-what-is-the-purpose-of-safearea-widget-in-flutter)

---

### Easy 15. Differentiate between mainaxisalignment and crossaxisalignment

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

- **`mainAxisAlignment`:** Aligns the children of a flex layout (Row or Column) along its primary axis. For a Row, this is horizontal. For a Column, this is vertical.
- **`crossAxisAlignment`:** Aligns children along the opposite (cross) axis. For a Row, this is vertical. For a Column, this is horizontal.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#easy-15-differentiate-between-mainaxisalignment-and-crossaxisalignment)

---

### Easy 16. What is the difference between container and sizedbox widget

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

- **`SizedBox`:** A lightweight widget used to define fixed dimensions or add empty spacing between widgets. It is cheap to render and supports a `const` constructor.
- **`Container`:** A heavier widget that combines painting, positioning, and sizing. It supports properties like decoration (borders, colors, shadows), padding, margins, and alignment. Use `SizedBox` instead of `Container` when only sizing or spacing is needed to optimize performance.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#easy-16-what-is-the-difference-between-container-and-sizedbox-widget)

---

### Easy 17. What do you mean by null aware operators

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

Null-aware operators in Dart simplify handling null values:
- **`??` (If-Null):** Returns the left operand if not null; otherwise, returns the right operand.
- **`?.` (Conditional Member Access):** Calls a method or accesses a property only if the object is not null.
- **`??=` (Null-Aware Assignment):** Assigns a value to a variable only if the variable is currently null.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#easy-17-what-do-you-mean-by-null-aware-operators)

---

### Easy 18. What is texteditingcontroller

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

`TextEditingController` is a class used to read, modify, and monitor text inputs in widgets like `TextField` or `TextFormField`. It allows you to: 
- Retrieve the current text.
- Pre-fill or clear text programmatically.
- Listen for real-time user input changes via a listener.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#easy-18-what-is-texteditingcontroller)

---

### Easy 19. What is an aspectratio widget used for

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

The `AspectRatio` widget forces its child widget to maintain a specific aspect ratio (the ratio of width to height), even if the parent constraints would otherwise dictate different dimensions. For example, `aspectRatio: 16 / 9` will maintain a widescreen box layout.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#easy-19-what-is-an-aspectratio-widget-used-for)

---

### Easy 20. What is assert used for in dart and flutter

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

An `assert` statement is a debugging tool used to enforce assumptions in code. If the condition inside an assertion evaluates to false, the program throws an error. Assertions are only executed in **debug mode** and are completely ignored in **release mode**, meaning they have zero impact on production performance.

```dart
assert(age >= 18, 'Must be an adult');
```

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#easy-20-what-is-assert-used-for-in-dart-and-flutter)

---

### Easy 21. How would you make http requests in the flutter framework

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

HTTP requests in Flutter are typically made using either:
1. **`http` package:** A simple, official Dart package for standard HTTP requests.
2. **`dio` package:** A powerful library that supports advanced features like interceptors, request cancellation, file downloading, and global configuration.

### Code Example

```dart
import 'dart:convert';
import 'package:http/http.dart' as http;

Future<void> fetchData() async {
  final response = await http.get('https://jsonplaceholder.typicode.com/posts');

  if (response.statusCode == 200) {
    // If the server did return a 200 OK response, then parse the JSON
    final data = json.decode(response.body);
    print(data);
  } else {
    // If the server did not return a 200 OK response, then throw an exception
    throw Exception('Failed to load data');
  }
}
```

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#easy-21-how-would-you-make-http-requests-in-the-flutter-framework)

---

### Easy 22. What technology is flutter built with

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

Flutter is built using three primary layers:
1. **Framework (Dart):** The high-level layer that contains the UI components, animations, layout mechanisms, and state management widgets. This is what developers interact with directly.
2. **Engine (C++):** The core layer that handles graphics rendering (via Impeller or Skia), text layout, file and network I/O, accessibility support, and the Dart runtime environment.
3. **Embedder (Platform-Specific):** The glue layer written in native languages (Java/C++ for Android, Objective-C/C++ for iOS, C++ for Windows) that allows Flutter to run on different operating systems and handle lifecycle events.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#easy-22-what-technology-is-flutter-built-with)

---

### Easy 23. What is the purpose of the initstate method in a statefulwidget

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

`initState()` is a lifecycle method called exactly once when a `StatefulWidget` is inserted into the widget tree. It is used to initialize variables, set up listeners (like streams or controllers), and fetch initial data from services. You must call `super.initState()` at the start of this method.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#easy-23-what-is-the-purpose-of-the-initstate-method-in-a-statefulwidget)

---

### Easy 24. What is the purpose of the dispose method in a statefulwidget

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

`dispose()` is a lifecycle method called when a `StatefulWidget` is permanently removed from the widget tree. It is used to clean up resources, such as closing streams, animation controllers, and text editing controllers, preventing memory leaks in the application. You must call `super.dispose()` at the end of the method.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#easy-24-what-is-the-purpose-of-the-dispose-method-in-a-statefulwidget)

---

### Easy 25. What is the difference between padding and margin in flutter

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

- **`Padding`:** Adds space *inside* the widget's border, separating the widget's content from its own border.
- **`Margin`:** Adds space *outside* the widget's border, separating the widget from its surrounding parent or sibling widgets.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#easy-25-what-is-the-difference-between-padding-and-margin-in-flutter)

---

### Easy 26. What is the purpose of the scaffold widget in flutter

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

The `Scaffold` widget implements the basic visual layout structure of Material Design. It acts as a container that provides standard UI slots for elements like an `AppBar` (top header), a `body` (main content), a `floatingActionButton` (action button), a `drawer` (side menu), and a `bottomNavigationBar`.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#easy-26-what-is-the-purpose-of-the-scaffold-widget-in-flutter)

---

### Easy 27. What is the purpose of the expanded widget in flutter

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

The `Expanded` widget wraps a child widget in a `Row`, `Column`, or `Flex` container, forcing the child to fill all the remaining available space along the main axis. If multiple children are expanded, the space is divided among them based on their `flex` factor values.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#easy-27-what-is-the-purpose-of-the-expanded-widget-in-flutter)

---

### Easy 28. What is the purpose of the singlechildscrollview widget in flutter

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

`SingleChildScrollView` is a widget that makes a single child widget scrollable. It is most useful for containers that might overflow on smaller screens (such as scrollable forms or setting lists) but do not have enough elements to justify a lazy-loading `ListView`.

### Code Example

```dart
SingleChildScrollView(
  child: Column(
    children: <Widget>[
      ListTile(title: Text('Item 1')),
      ListTile(title: Text('Item 2')),
      ListTile(title: Text('Item 3')),
      // Add more items here...
    ],
  ),
);
```

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#easy-28-what-is-the-purpose-of-the-singlechildscrollview-widget-in-flutter)

---

### Easy 29. What is the purpose of the stack widget in flutter

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

The `Stack` widget allows you to position children on top of each other, overlapping them from back to front (like layers). Children of a `Stack` can be styled as: 
- **Unpositioned:** Sized and positioned normally.
- **Positioned:** Wrapped in a `Positioned` widget to place them at absolute coordinates relative to the Stack's boundaries (e.g., `top: 10`, `right: 5`).

### Code Example

```dart
Stack(
  children: [
    Image.network('https://picsum.photos/250?image=9'),
    Center(child: Text('Hello, World!'),
  ],
),
```

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#easy-29-what-is-the-purpose-of-the-stack-widget-in-flutter)

---

### Easy 30. What is a theme in flutter

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

A `Theme` in Flutter is a way to define and apply global colors, typography, and component styles across your entire application. By wrapping your app with a `Theme` widget (typically inside `MaterialApp.theme`), descendant widgets can automatically inherit and reference uniform colors (like `Theme.of(context).primaryColor`).

### Code Example

```dart
MaterialApp(
  theme: ThemeData(
    primaryColor: Colors.blue,
    accentColor: Colors.orange,
    textTheme: TextTheme(
      headline1: TextStyle(fontSize: 36, fontWeight: FontWeight.bold),
      bodyText1: TextStyle(fontSize: 18),
    ),
  ),
),
```

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#easy-30-what-is-a-theme-in-flutter)

---

### Easy 31. What is the purpose of the visibility widget in flutter

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

The `Visibility` widget controls whether its child widget is visible on the screen. It supports multiple modes:
- **`visible: false`:** Hides the widget. By default, it replaces the child with a zero-size box (removing it from layout).
- **`maintainState: true`, `maintainSize: true`:** Hides the widget visually but keeps it active in the layout, preserving its space and state so surrounding elements don't shift.

### Code Example

```dart
Visibility(
  visible: true, // currently visible, set to `false` to disappear 
  child: Text(
    'Hello, World!',
    style: TextStyle(fontSize: 24),
  ),
),
```

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#easy-31-what-is-the-purpose-of-the-visibility-widget-in-flutter)

---

### Easy 32. How do you navigate between screens in flutter

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

Navigation in Flutter is managed by the `Navigator` class, which uses a stack structure (Last-In, First-Out):
- **`Navigator.push()`:** Pushes a new route onto the stack, displaying a new screen.
- **`Navigator.pop()`:** Pops the top route off the stack, returning to the previous screen.
Routes can be defined on the fly using `MaterialPageRoute` or pre-configured as static string paths in the `MaterialApp` widget (named routes).

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#easy-32-how-do-you-navigate-between-screens-in-flutter)

---

### Easy 33. What is a modal bottom sheet in flutter

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

A modal bottom sheet is a Material Design overlay widget that rises from the bottom of the screen, partially covering the content. It is displayed using `showModalBottomSheet()` and is typically used to present a menu, a list of actions, or small inputs without navigating away from the current page.

### Code Example

```dart
showModalBottomSheet(
  context: context,
  builder: (BuildContext context) {
    return Container(
      // WRITE YOUR CODE HERE
    );
  },
);
```

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#easy-33-what-is-a-modal-bottom-sheet-in-flutter)

---

### Easy 34. How do you use the positioned widget in flutter

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

The `Positioned` widget must be used as a direct child of a `Stack`. It allows you to place a widget at absolute coordinates relative to the Stack's boundaries by specifying parameters like `top`, `bottom`, `left`, `right`, `width`, and `height`.

### Code Example

```dart
Stack(
  children: [
    Positioned(
      left: 10,
      top: 10,
      child: Text('Hi there!'),
    ),
    Positioned(
      right: 10,
      bottom: 10,
      child: Text('Bye there!'),
    ),
  ],
),
```

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#easy-34-how-do-you-use-the-positioned-widget-in-flutter)

---

### Easy 35. How do you pass data between screens in flutter

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

Data can be passed between screens in Flutter using two main methods:
1. **Constructor Injection:** Pass data directly into the constructor of the destination screen when navigating:
   ```dart
   Navigator.push(context, MaterialPageRoute(builder: (_) => DetailScreen(data: myData)));
   ```
2. **Route Arguments:** Pass data as an argument when navigating with named routes, retrieving it on the destination screen via `ModalRoute.of(context)!.settings.arguments`.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#easy-35-how-do-you-pass-data-between-screens-in-flutter)

---

### Easy 36. What is the purpose of the navigator class in flutter

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

`Navigator` is a widget that manages a stack of child widgets (screens). It tracks the screen navigation history, providing standard operations like `push` to navigate forward, `pop` to navigate backward, and `pushReplacement` to swap the current screen, implementing standard app navigation patterns.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#easy-36-what-is-the-purpose-of-the-navigator-class-in-flutter)

---

### Easy 37. What is the purpose of the fittedbox widget in flutter

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

The `FittedBox` widget scales and positions its child widget to fit within its allocated parent space according to a specified `BoxFit` behavior (such as containment or filling). It is highly useful for preventing text or layout elements from overflowing on smaller screen boundaries.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#easy-37-what-is-the-purpose-of-the-fittedbox-widget-in-flutter)

---

### Easy 38. What is the difference between cupertino and material design in flutter

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

Flutter supports two design languages out-of-the-box:
- **Material Design:** Google's standard visual design system, designed for Android and web apps (widgets like `Scaffold`, `AppBar`, `ElevatedButton`).
- **Cupertino:** Apple's human interface guidelines, designed to look and feel like iOS (widgets like `CupertinoPageScaffold`, `CupertinoNavigationBar`, `CupertinoButton`).

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#easy-38-what-is-the-difference-between-cupertino-and-material-design-in-flutter)

---

### Easy 39. What is the purpose of the material design icons package in flutter

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

The Material Design Icons package in Flutter provides pre-compiled vector icons that conform to Google's Material Design standard. Using them is lightweight and scale-invariant because they are loaded from a compiled font file (`Icons.add`, `Icons.home`, etc.).

### Code Example

```dart
import 'package:flutter/material.dart';
import 'package:material_design_icons_flutter/material_design_icons_flutter.dart';

class MyApp extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      appBar: AppBar(
        title: Text('My App'),
      ),
      body: Center(
        child: Icon(MdiIcons.home),
      ),
    );
  }
}
```

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#easy-39-what-is-the-purpose-of-the-material-design-icons-package-in-flutter)

---

### Easy 40. How doobjectdynamic andvardiffer in dart

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Easy

- **`Object`:** The base class for all Dart objects (except null). Variables declared as `Object` have compile-time type safety; you can only call methods defined on the `Object` class unless you perform an explicit cast.
- **`dynamic`:** Disables static compile-time type checking. You can call any method or property on a `dynamic` variable; type mismatches are caught only during runtime (which can cause crashes).
- **`var`:** A local keyword that tells the compiler to automatically infer the variable's type based on its initial assignment value. Once inferred, the type cannot be changed.

### Code Example

```dart
Object obj = "Hello";
```

```dart
dynamic obj = "Hello"; // obj.length; (no type safety, but flexible)
```

```dart
var obj = "Hello"; // (obj is inferred as String)
```

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#easy-40-how-doobjectdynamic-andvardiffer-in-dart)

---


## Medium Questions

### Medium 1. What is buildcontext in flutter and why is it needed

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

`BuildContext` represents a widget's location in the widget tree. It is passed to build methods and is needed to:
1. **Locate widgets:** Resolve where a widget is relative to others.
2. **Look up themes and inherited widgets:** Access data higher up in the tree (e.g., `Theme.of(context)`).
3. **Handle navigation and dialogs:** Provide the context required by functions like `Navigator.push` or `showDialog`.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#medium-1-what-is-buildcontext-in-flutter-and-why-is-it-needed)

---

### Medium 2. What are different build modes in flutter

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

Flutter supports three build modes:
1. **Debug:** Optimized for rapid development. Features like Hot Reload are enabled, and full debugging tools are supported. Execution is slower.
2. **Profile:** Used to analyze performance. It maintains enough debugging capabilities to profile app behavior while running close to native speed.
3. **Release:** Optimized for deployment. The code is fully compiled and minified, debugging features are stripped out, and the app size is minimized for maximum speed.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#medium-2-what-are-different-build-modes-in-flutter)

---

### Medium 3. What is the difference between widgetsapp and materialapp in flutter

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

- **`WidgetsApp`:** A basic, custom-looking foundation widget. It includes features like navigation, routing, and basic app structuring, but has no pre-defined visual styling or design language.
- **`MaterialApp`:** Built on top of `WidgetsApp`. It configures your app to conform to Google's Material Design system, adding elements like themes, standard page transitions, and components (e.g., `Scaffold` and `AppBar`).

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#medium-3-what-is-the-difference-between-widgetsapp-and-materialapp-in-flutter)

---

### Medium 4. What are statefulwidget lifecycle methods explain briefly

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

The lifecycle of a `StatefulWidget` consists of the following key steps:
1. **`createState()`:** Called to create the mutable state object.
2. **`initState()`:** Called once when the state is inserted into the tree. Ideal for initialization.
3. **`didChangeDependencies()`:** Called right after `initState` or when an inherited dependency changes.
4. **`build()`:** Called to render the widget tree.
5. **`didUpdateWidget()`:** Called when the parent widget changes configuration and passes new properties.
6. **`setState()`:** Notifies the framework to rebuild the widget.
7. **`deactivate()`:** Called when the state is temporarily removed from the tree.
8. **`dispose()`:** Called when the state is permanently destroyed.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#medium-4-what-are-statefulwidget-lifecycle-methods-explain-briefly)

---

### Medium 5. What are keys and why do we need them

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

Keys are unique identifiers for widgets. Flutter uses them to preserve the state of `StatefulWidget`s when they move around or change position in the widget tree. They are essential when working with collections of widgets of the same type (like lists) to ensure the framework updates the correct elements.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#medium-5-what-are-keys-and-why-do-we-need-them)

---

### Medium 6. What is the difference between expanded and flexible widget

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

- **`Flexible`:** Allows a child widget of a `Row` or `Column` to fit within the available space. By default, it lets the child shrink or grow, occupying only the space it needs.
- **`Expanded`:** A subclass of `Flexible` that forces the child widget to fill all the remaining available space along the main axis.

### Code Example

```dart
Column(children: [
  Row(
    children: [_ExpandedWidget(), _FlexibleWidget()],
  ),
  Row(
    children: [_ExpandedWidget(), _ExpandedWidget()],
  ),
  Row(
    children: [_FlexibleWidget(), _FlexibleWidget()],
  ),
]),
```

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#medium-6-what-is-the-difference-between-expanded-and-flexible-widget)

---

### Medium 7. What is the extension method in dart

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

Extension methods allow you to add new features or methods to existing classes or libraries without modifying the original code or subclassing. They are highly useful for extending Dart core libraries or Flutter classes.

```dart
extension StringExtensions on String {
  bool get isValidEmail => contains('@');
}

// Usage
print('test@mail.com'.isValidEmail); // true
```

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#medium-7-what-is-the-extension-method-in-dart)

---

### Medium 8. Explain the mounted property how is it important and when to use it

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

The `mounted` property is a boolean flag that indicates whether a widget's state object is currently in the widget tree. It is crucial to check `if (mounted)` before calling `setState()` inside asynchronous operations (like network fetches) to avoid errors that occur if the widget has already been destroyed.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#medium-8-explain-the-mounted-property-how-is-it-important-and-when-to-use-it)

---

### Medium 9. What is sound null safety

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

Sound null safety in Dart makes types non-nullable by default. If you declare a variable, it cannot hold a `null` value unless you explicitly mark it as nullable using a question mark `?`. This allows the compiler to detect and prevent null pointer exceptions during compilation rather than at runtime.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#medium-9-what-is-sound-null-safety)

---

### Medium 10. What are mixins how to use them

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

A mixin is a class that allows other classes to reuse its methods and properties without subclassing (inheritance). In Dart, a class can mix in multiple classes using the `with` keyword.

```dart
mixin Swimmer {
  void swim() => print('Swimming...');
}

class Duck extends Animal with Swimmer {}
```
To restrict which classes can use a mixin, use the `on` keyword (e.g., `mixin Flyer on Bird`).

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#medium-10-what-are-mixins-how-to-use-them)

---

### Medium 11. What is applifecyclestate

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

`AppLifecycleState` is an enum that represents the runtime state of a Flutter application. The main states are:
- **`resumed`:** The app is in the foreground, visible, and responding to user input.
- **`inactive`:** The app is visible but not receiving input (e.g., phone call overlay, system dialogs).
- **`paused`:** The app is in the background and not visible.
- **`detached`:** The app is still running a Dart engine but is disconnected from any host views.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#medium-11-what-is-applifecyclestate)

---

### Medium 12. What is the difference between networkimage and imagenetwork in flutter

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

- **`NetworkImage`:** A low-level class (an `ImageProvider`) that fetches an image from the network. It does not display anything directly but is passed to widgets like `DecorationImage` or `Image`.
- **`Image.network()`:** A convenience widget that displays an image from a URL on the screen. Under the hood, it uses `NetworkImage` as its provider.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#medium-12-what-is-the-difference-between-networkimage-and-imagenetwork-in-flutter)

---

### Medium 13. Explain async await and future

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

- **`Future`:** Represents a delayed computation or result that will complete in the future.
- **`async`:** A keyword used to mark a function that performs asynchronous work and returns a Future.
- **`await`:** A keyword used to pause execution of an async function until a Future resolves, allowing asynchronous code to be written sequentially.

```dart
Future<String> fetchData() async {
  return await http.get('url');
}
```

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#medium-13-explain-async-await-and-future)

---

### Medium 14. What is resizetoavoidbottominset when should we use it

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

`resizeToAvoidBottomInset` is a boolean property of the `Scaffold` widget. When set to `true` (default), the Scaffold automatically shrinks its body height when the on-screen keyboard appears, preventing the keyboard from covering inputs. Set it to `false` if you want your layout to remain static and overlap behind the keyboard.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#medium-14-what-is-resizetoavoidbottominset-when-should-we-use-it)

---

### Medium 15. What is animation and animationcontroller

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

- **`Animation`:** A class that generates a sequence of values (typically between 0.0 and 1.0) over a specific time duration to drive a transition.
- **`AnimationController`:** A special `Animation` class that controls the animation. It allows you to play, pause, reverse, and stop the animation, and coordinates frame updates via the screen's refresh rate (vsync).

### Code Example

```dart
class MyAnimation extends StatefulWidget {
  @override
  _MyAnimationState createState() => _MyAnimationState();
}

class _MyAnimationState extends State<MyAnimation>
    with SingleTickerProviderStateMixin {
  AnimationController _controller;
  Animation<double> _animation;

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(
      duration: Duration(seconds: 2),
      vsync: this,
    );
    _animation = Tween<double>(begin: 0, end: 300).animate(_controller)
      ..addListener(() {
        setState(() {});
      });
  }

  @override
  void dispose() {
    _controller.dispose();
    super.dispose();
  }

  @override
  Widget build(BuildContext context) {
    return Container(
      height: _animation.value,
      width: _animation.value,
      child: FlutterLogo(),
    );
  }
}
```

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#medium-15-what-is-animation-and-animationcontroller)

---

### Medium 16. Differentiate between stream and future in flutter

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

- **`Future`:** Represents a single asynchronous event or response that will arrive in the future (one-time completion).
- **`Stream`:** Represents a sequence of asynchronous events or data packets that arrive over time (multiple events, like a web socket stream or button clicks).

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#medium-16-differentiate-between-stream-and-future-in-flutter)

---

### Medium 17. Can you explain the process of creating custom widgets in flutter

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

To create custom widgets in Flutter, developers use composition (combining existing widgets) rather than subclassing. The standard process is:
1. Extend `StatelessWidget` or `StatefulWidget`.
2. Pass configuration parameters via the constructor.
3. Override the `build` method to return a combination of built-in widgets (like Container, Padding, Column).

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#medium-17-can-you-explain-the-process-of-creating-custom-widgets-in-flutter)

---

### Medium 18. What is typedef in dart

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

A `typedef` (type alias) in Dart creates a user-friendly alias for a complex type definition, commonly function signatures or long generic types. This makes the code cleaner, more readable, and easier to maintain.

```dart
typedef OnValueChanged = void Function(int newValue);

// Usage
final OnValueChanged callback;
```

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#medium-18-what-is-typedef-in-dart)

---

### Medium 19. What is futurebuilder in flutter and how is it used to build dynamic ui

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

`FutureBuilder` is a widget that listens to a `Future` and builds its UI based on the latest state of that Future. It runs through three main states using `AsyncSnapshot`:
1. **Waiting:** Displays a loading spinner while the Future is running.
2. **Done with Error:** Renders an error message if the Future fails.
3. **Done with Data:** Displays the successful result when the Future resolves.

### Code Example

```dart
Future<List<String>> _fetchData() async {
  // Simulate fetching data from a server
  return Future.delayed(Duration(seconds: 2), () => ["Item 1", "Item 2", "Item 3"]);
}

@override
Widget build(BuildContext context) {
  return FutureBuilder<List<String>>(
    future: _fetchData(),
    builder: (context, snapshot) {
      if (snapshot.hasData) {
        return ListView.builder(
          itemCount: snapshot.data.length,
          itemBuilder: (context, index) {
            return Text(snapshot.data[index]);
          },
        );
      } else if (snapshot.hasError) {
        return Text("Error: ${snapshot.error}");
      }
      return CircularProgressIndicator();
    },
  );
}
```

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#medium-19-what-is-futurebuilder-in-flutter-and-how-is-it-used-to-build-dynamic-ui)

---

### Medium 20. How do you handle exceptions in flutter and what strategies have you used

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

Exceptions in Flutter can be handled at multiple levels:
1. **Try-Catch Blocks:** Handle local synchronous or asynchronous code blocks.
2. **`FlutterError.onError`:** Intercept and log uncaught Flutter framework UI errors.
3. **`PlatformDispatcher.instance.onError`:** Intercept asynchronous Dart zone errors.
4. **Services:** Integrate crash reporting SDKs like Firebase Crashlytics to monitor issues in production.

### Code Example

```dart
try {
  // Code that might throw an exception
} on Exception catch (e) {
  // Code that is executed when an exception is caught
  print("Caught exception: $e");
}
```

```dart
try {
  // Code that might throw an exception
} on SocketException catch (e) {
  // Code that is executed when a SocketException is caught
  print("Caught SocketException: $e");
  // Retry the operation
} on FormatException catch (e) {
  // Code that is executed when a FormatException is caught
  print("Caught FormatException: $e");
  // Show an error message to the user
} catch (e) {
  // Code that is executed when any other exception is caught
  print("Caught exception: $e");
  // Log the exception for debugging purposes
}
```

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#medium-20-how-do-you-handle-exceptions-in-flutter-and-what-strategies-have-you-used)

---

### Medium 21. What are devtools in flutter

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

Flutter DevTools is a suite of performance and debugging tools. It helps developers:
- Inspect the widget tree and modify layouts in real-time (Flutter Inspector).
- Analyze CPU usage and trace memory leaks.
- Inspect network traffic and monitor API response times.
- Profile app startup performance and view GPU render cycles.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#medium-21-what-are-devtools-in-flutter)

---

### Medium 22. What is factory constructor

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

A `factory` constructor is a constructor in Dart that does not always create a new instance of its class. It is useful for:
- Returning an existing cached instance (Singleton pattern).
- Instantiating a specific subclass rather than the parent class.
- Initializing an instance from raw data (e.g., parsing JSON via `factory Class.fromJson`).

### Code Example

```dart
class Rectangle {
  final double width;
  final double height;

  Rectangle(this.width, this.height);

  factory Rectangle.square(double side) {
    return Rectangle(side, side);
  }
}
```

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#medium-22-what-is-factory-constructor)

---

### Medium 23. Explain singleton class in flutter

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

A Singleton is a design pattern that ensures a class has only one instance and provides a global access point to it. In Dart, it is implemented using a private constructor and a static instance returned via a factory constructor:

```dart
class DatabaseService {
  DatabaseService._privateConstructor();
  static final DatabaseService instance = DatabaseService._privateConstructor();
  
  factory DatabaseService() => instance;
}
```

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#medium-23-explain-singleton-class-in-flutter)

---

### Medium 24. What is the event loop

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

Dart is a single-threaded language. It uses an **Event Loop** to execute asynchronous tasks. The event loop continuously processes tasks from two FIFO queues:
1. **Microtask Queue:** Holds internal system tasks. Tasks here are run first until the queue is completely empty.
2. **Event Queue:** Holds external events like I/O operations, timers, tap gestures, and drawing frames.
When both queues are empty, the event loop waits for new events.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#medium-24-what-is-the-event-loop)

---

### Medium 25. What is the difference between provider vs inheritedwidget

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

- **`InheritedWidget`:** The low-level, built-in Flutter class for sharing data down the widget tree. It requires a lot of boilerplate code and is harder to manage for complex states.
- **`Provider`:** A popular, high-level wrapper built on top of `InheritedWidget`. It simplifies state management by drastically reducing boilerplate, improving readability, and offering features like lazy loading and clean resource allocation.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#medium-25-what-is-the-difference-between-provider-vs-inheritedwidget)

---

### Medium 26. What is a globalkey in flutter

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

A `GlobalKey` is a unique key across the entire application. Unlike a local key, a `GlobalKey` allows a widget to be moved anywhere in the tree without losing its state. It also grants access to the state (`State`) and layout parameters (`RenderObject`) of the associated widget from anywhere in the codebase. Because they are computationally expensive, use them sparingly.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#medium-26-what-is-a-globalkey-in-flutter)

---

### Medium 27. How do you handle user input in flutter

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

Flutter handles user input using various specialized widgets:
1. **`TextField` / `TextFormField`:** Manage text entry and input validation.
2. **`GestureDetector`:** Detects tap, double tap, drag, long press, and zoom gestures on any child widget.
3. **`InkWell`:** Works like `GestureDetector` but adds visual material ripple feedback when tapped.
4. **Selection Widgets:** Standard elements like `Checkbox`, `Switch`, `Radio`, and `Slider` handle toggle and range inputs.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#medium-27-how-do-you-handle-user-input-in-flutter)

---

### Medium 28. What is the purpose of the layoutbuilder widget in flutter

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

`LayoutBuilder` is a widget that reads the constraints passed down from its parent widget and builds its child widget accordingly. It provides a `BoxConstraints` object containing the maximum and minimum width and height available, making it essential for building responsive UIs that adapt to different screen sizes.

### Code Example

```dart
LayoutBuilder(
  builder: (BuildContext context, BoxConstraints constraints) {
    return Container(
      width: constraints.maxWidth * 0.5,
      height: constraints.maxHeight * 0.5,
      child: Text('This widget will take up 50% of the available space'),
    );
  },
);
```

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#medium-28-what-is-the-purpose-of-the-layoutbuilder-widget-in-flutter)

---

### Medium 29. How do you use the valuenotifier class in flutter

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

`ValueNotifier` is a lightweight class that stores a single value and notifies its listeners when that value changes. To render updates on the screen without triggering a full page `setState()`, it is paired with a `ValueListenableBuilder` widget, which only rebuilds the specific widget that depends on the value.

```dart
final ValueNotifier<int> counter = ValueNotifier<int>(0);
// To change value
counter.value++;
```

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#medium-29-how-do-you-use-the-valuenotifier-class-in-flutter)

---

### Medium 30. What is a mediaquery in flutter

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

`MediaQuery` is a widget that provides information about the size, orientation, and layout settings of the current device screen (e.g., width, height, aspect ratio, safe padding). Calling `MediaQuery.of(context).size` allows developers to build responsive widgets that adjust their sizes based on the screen width or orientation.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#medium-30-what-is-a-mediaquery-in-flutter)

---

### Medium 31. What is the purpose of the didupdatewidget method in a statefulwidget

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

`didUpdateWidget()` is a StatefulWidget lifecycle method called whenever the parent widget rebuilds and passes new configuration parameters to the child widget. It gives you access to the `oldWidget` parameter, allowing you to compare old and new properties to trigger specific side effects or restart animations.

### Code Example

```dart
class MyWidget extends StatefulWidget {
  final String data;

  MyWidget({required this.data});

  @override
  _MyWidgetState createState() => _MyWidgetState();
}

class _MyWidgetState extends State<MyWidget> {
  String _data = '';

  @override
  void initState() {
    super.initState();
    _data = widget.data;
  }

  @override
  void didUpdateWidget(covariant MyWidget oldWidget) {
    super.didUpdateWidget(oldWidget);
    if (widget.data != oldWidget.data) {
      setState(() {
        _data = widget.data;
      });
    }
  }

  @override
  Widget build(BuildContext context) {
    return Text(_data);
  }
}
```

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#medium-31-what-is-the-purpose-of-the-didupdatewidget-method-in-a-statefulwidget)

---

### Medium 32. What is the purpose of the animatedbuilder widget in flutter

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

`AnimatedBuilder` is a specialized widget that optimizes animation performance. It rebuilds only its builder subtree when an animation ticks, avoiding rebuilding other static child widgets that do not depend on the animation. This separation of concerns improves rendering efficiency.

### Code Example

```dart
class MyWidget extends StatefulWidget {...

class _MyWidgetState extends State<MyWidget> with SingleTickerProviderStateMixin {
  late AnimationController _controller;
  late Animation<double> _animation;

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(
      duration: const Duration(seconds: 1),
      vsync: this,
    );
    _animation = Tween<double>(begin: 0, end: 1).animate(_controller);
    _controller.repeat(reverse: true);
  }

  @override
  void dispose() {
    _controller.dispose();
    super.dispose();
  }

  @override
  Widget build(BuildContext context) {
    return AnimatedBuilder(
      animation: _animation,
      builder: (context, child) {
        return Opacity(
          opacity: _animation.value,
          child: Container( ... ),
        );
      },
    );
  }
}
```

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#medium-32-what-is-the-purpose-of-the-animatedbuilder-widget-in-flutter)

---

### Medium 33. What is the purpose of the animatedswitcher widget in flutter

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

`AnimatedSwitcher` is a widget that automatically animates transitions when its child widget changes (e.g., swapping a Text widget for an Image widget). It detects changes based on the widget type or key, applying smooth cross-fades or custom animations during the swap.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#medium-33-what-is-the-purpose-of-the-animatedswitcher-widget-in-flutter)

---

### Medium 34. What is state management in flutter

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

State management is the practice of managing how data is stored, updated, and synchronized across widgets in a Flutter application. Since Flutter UIs are declarative (built by rebuilding when state changes), choosing a state management solution (such as Provider, Riverpod, BLoC, or MobX) ensures clean architecture, separation of logic, and efficient updates.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#medium-34-what-is-state-management-in-flutter)

---

### Medium 35. How do you implement a draggable widget in flutter

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

A draggable widget is implemented in Flutter using three main classes:
1. **`Draggable`:** The widget that the user can press and drag across the screen.
2. **`DragTarget`:** The landing area widget that accepts or rejects incoming dragged data.
3. **`LongPressDraggable`:** A subclass of `Draggable` that requires a long press to start dragging.

### Code Example

```dart
Draggable<int>(
  data: 1,
  feedback: Material(
    color: Colors.transparent,
    child: Icon(Icons.access_alarm, size: 50),
  ),
  childWhenDragging: Container(),
  child: Icon(Icons.access_alarm),
)
```

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#medium-35-how-do-you-implement-a-draggable-widget-in-flutter)

---

### Medium 36. How do you provide accessibility when developing flutter apps do you at all

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

Flutter provides high-quality accessibility support natively. Best practices include:
- Wrapping decorative images in `Semantics(excludeSemantics: true)` or leaving the semantic label empty.
- Providing descriptive text labels for widgets (like buttons) using the `Semantics` widget.
- Ensuring the layout has adequate contrast ratios and conforms to system text scaling settings.
- testing with screen readers (TalkBack on Android, VoiceOver on iOS).

### Code Example

```dart
Semantics(
  label: 'Submit button',
  child: ElevatedButton(onPressed: () {}, child: Text('Submit')),
);
```

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#medium-36-how-do-you-provide-accessibility-when-developing-flutter-apps-do-you-at-all)

---

### Medium 37. How to create a list with persistent headers

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

To create a scrollable list with persistent headers (sticky headers), you typically use:
1. **`CustomScrollView`** containing **`SliverPersistentHeader`** widgets.
2. Implementing a custom delegate that extends `SliverPersistentHeaderDelegate` to define the header size and appearance when pinned.
3. Alternatively, importing third-party helper packages like `flutter_sticky_headers`.

### Code Example

```dart
class PersistentHeaderList extends StatelessWidget {
  @override
  Widget build(BuildContext context) {
    return Scaffold(
      body: CustomScrollView(
        slivers: <Widget>[
          SliverPersistentHeader(
            delegate: _MyPersistentHeaderDelegate(),
            pinned: true, // Makes the header sticky
          ),
          SliverList(
            delegate: SliverChildBuilderDelegate(
              (BuildContext context, int index) {
                return ListTile(title: Text('Item $index'));
              },
              childCount: 100,
            ),
          ),
        ],
      ),
    );
  }
}

class _MyPersistentHeaderDelegate extends SliverPersistentHeaderDelegate {
  @override
  double get maxExtent => 100.0;
  @override
  double get minExtent => 60.0;

  @override
  Widget build(BuildContext context, double shrinkOffset, bool overlapsContent) {
    return Container(
      color: Colors.blue,
      child: Text('Persistent Header'),
    );
  }

  @override
  bool shouldRebuild(covariant SliverPersistentHeaderDelegate oldDelegate) => false;
}
```

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#medium-37-how-to-create-a-list-with-persistent-headers)

---

### Medium 38. Explain what a ticker is in flutter

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

A `Ticker` is a class in Flutter that calls its callback function once per frame (typically 60 or 120 times per second). Animation controllers use tickers to update animation values incrementally. To associate a StatefulWidget with a Ticker, classes mix in `SingleTickerProviderStateMixin` (for a single ticker) or `TickerProviderStateMixin` (for multiple tickers).

### Code Example

```dart
class MyAnimatedWidget extends StatefulWidget {
  @override
  _MyAnimatedWidgetState createState() => _MyAnimatedWidgetState();
}

class _MyAnimatedWidgetState extends State<MyAnimatedWidget> with TickerProviderStateMixin {
  late Ticker _ticker;

  @override
  void initState() {
    super.initState();
    _ticker = createTicker((elapsed) {
      print('Time elapsed: $elapsed');
    });
    _ticker.start();  // Starts the ticker
  }

  @override
  void dispose() {
    _ticker.dispose(); // Clean up the ticker
    super.dispose();
  }

  @override
  Widget build(BuildContext context) {
    return Container();
  }
}
```

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#medium-38-explain-what-a-ticker-is-in-flutter)

---

### Medium 39. What are the various kinds of streams present in flutter

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

Dart has two types of Streams:
1. **Single-Subscription Stream:** Allows only a single listener during its lifetime. If you try to listen to it a second time, it throws an error. Good for sequential events (like reading a file stream).
2. **Broadcast Stream:** Allows multiple listeners simultaneously. Useful for global events (like controller state updates or sensor events). Created by calling `stream.asBroadcastStream()`.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#medium-39-what-are-the-various-kinds-of-streams-present-in-flutter)

---

### Medium 40. What are the differences between jit and aot

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

- **JIT (Just-In-Time) Compilation:** Compiles code on-the-fly during runtime. Used in Flutter's development build mode to enable fast developer iteration and Hot Reload capabilities.
- **AOT (Ahead-Of-Time) Compilation:** Compiles code to native machine code *before* execution. Used in release mode to speed up application startup times and ensure native execution speed.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#medium-40-what-are-the-differences-between-jit-and-aot)

---

### Medium 41. How do mixins differ from interfaces in dart

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Medium

- **Mixins:** Provide concrete code implementation (both method declarations and actual bodies) that can be shared across multiple unrelated classes using the `with` keyword, avoiding class hierarchy constraints.
- **Interfaces:** Define a blueprint (contract) with abstract method signatures that class subclasses must implement using the `implements` keyword. Dart has no explicit interface keyword; every class implicitly defines its own interface.

### Code Example

```dart
mixin Walker {
  void walk() => print("Walking");
}

class Person with Walker {
  // Person can now use the walk() method
}
```

```dart
class Animal {
  void eat();
}

class Dog implements Animal {
  @override
  void eat() => print("Dog eating");
}
```

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#medium-41-how-do-mixins-differ-from-interfaces-in-dart)

---


## Hard Questions

### Hard 1. What are slivers

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Hard

A **sliver** is a portion of a scrollable area that manages its own layout. Under the hood, scrollable widgets like `ListView` and `GridView` are built using slivers. Using slivers directly (via `CustomScrollView`) allows you to create advanced, custom scrolling effects like collapsible app bars, sticky headers, and mixed grid-list layouts.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#hard-1-what-are-slivers)

---

### Hard 2. What is inheritedwidget in flutter

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Hard

`InheritedWidget` is a special class that propagates data down the widget tree. Any descendant widget in the subtree can read data from an `InheritedWidget` without having it passed explicitly through parameters. When the data inside an `InheritedWidget` changes, it automatically notifies and rebuilds dependent descendant widgets.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#hard-2-what-is-inheritedwidget-in-flutter)

---

### Hard 3. What is flutter tree shaking

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Hard

Tree shaking is a compiler optimization technique used during production release compilation. It analyzes the source code and automatically removes unused code, variables, and imported libraries. This helps reduce the final binary size of the Flutter application.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#hard-3-what-is-flutter-tree-shaking)

---

### Hard 4. What is vsync explain

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Hard

`vsync` (Vertical Synchronization) is a parameter passed to `AnimationController`. It coordinates the controller to generate animation ticks only when the screen is ready to paint a new frame. This prevents off-screen animations from consuming CPU resources, reducing battery usage and screen tearing.

### Code Example

```dart
class MyAnimation extends StatefulWidget {
  @override
  _MyAnimationState createState() => _MyAnimationState();
}

class _MyAnimationState extends State<MyAnimation>
    with SingleTickerProviderStateMixin {
  AnimationController _controller;
  Animation<double> _animation;

  @override
  void initState() {
    super.initState();
    _controller = AnimationController(
      duration: Duration(seconds: 2),
      vsync: this,
    );
    _animation = Tween<double>(begin: 0, end: 300).animate(_controller)
      ..addListener(() {
        setState(() {});
      });
  }

  @override
  void dispose() {
    _controller.dispose();
    super.dispose();
  }

  @override
  Widget build(BuildContext context) {
    return Container(
      height: _animation.value,
      width: _animation.value,
      child: FlutterLogo(),
    );
  }
}
```

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#hard-4-what-is-vsync-explain)

---

### Hard 5. What is isolate in flutter

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Hard

An `Isolate` is Dart's model for concurrency. Unlike traditional multi-threading where threads share memory, each Dart Isolate has its own private memory heap and a single event loop. Because they do not share memory, isolates cannot cause resource locks or race conditions. Communication between isolates is achieved exclusively via message passing using `SendPort` and `ReceivePort`.

### Code Example

```dart
import 'dart:isolate';

void backgroundTask(SendPort sendPort) {
  // Code that runs in the background isolate
}

void main() {
  final receivePort = ReceivePort();
  Isolate.spawn(backgroundTask, receivePort.sendPort);
}
```

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#hard-5-what-is-isolate-in-flutter)

---

### Hard 6. Can you explain the process of testing a flutter app

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Hard

Testing a Flutter app involves three main categories:
1. **Unit Tests:** Verify individual functions, classes, and logic in isolation. Runs fast.
2. **Widget Tests:** Verify the UI layout and interactivity of a single widget without a device. Runs in a simulated environment.
3. **Integration Tests:** Test the entire app on a real device or emulator to verify end-to-end user flows and native integrations.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#hard-6-can-you-explain-the-process-of-testing-a-flutter-app)

---

### Hard 7. What is a custompainter in flutter

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Hard

`CustomPainter` is a low-level Flutter class used to draw custom shapes, paths, lines, and text directly onto a canvas. To implement it, you extend `CustomPainter`, override the `paint` method (to define what to draw using canvas drawing functions), and override the `shouldRepaint` method (to determine if the painting should update when values change). It is rendered inside a `CustomPaint` widget.

### Code Example

```dart
// Custom Painter
class RectanglePainter extends CustomPainter {
  @override
  void paint(Canvas canvas, Size size) {
    final paint = Paint()
      ..color = Colors.blue
      ..style = PaintingStyle.fill;
    final rect = Rect.fromLTWH(0, 0, size.width, size.height);
    canvas.drawRect(rect, paint);
  }

  @override
  bool shouldRepaint(RectanglePainter oldDelegate) => false;
}

// How to use the CustomPainter using CustomPaint widget
CustomPaint(
  painter: RectanglePainter(),
  size: Size(200, 200), // defines the sixe of the canvas
),
```

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#hard-7-what-is-a-custompainter-in-flutter)

---

### Hard 8. Explain how you will deploy a flutter app to the google playapp store

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Hard

Deploying a Flutter app involves:
1. **Android (Google Play Store):** Register your app in the Google Play Console, configure digital signing (generate keystore), update launcher icons, run `flutter build appbundle` to generate a release bundle, and upload it to Google Play Console.
2. **iOS (App Store):** Register on App Store Connect, configure provisioning profiles and certificates in Xcode, run `flutter build ipa` to bundle the app, and upload it using Transporter or Xcode.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#hard-8-explain-how-you-will-deploy-a-flutter-app-to-the-google-playapp-store)

---

### Hard 9. What are the advantages of a flutter inspector

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Hard

The Flutter Inspector is a tool within DevTools that helps developers view and debug layouts. Its key advantages include:
- Visualizing the widget tree layout details.
- Using 'Select Widget Mode' to tap an element on the screen and inspect its properties.
- Highlighting layout errors like overflows.
- Toggling debug paint boxes to see margins and paddings.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#hard-9-what-are-the-advantages-of-a-flutter-inspector)

---

### Hard 10. List the responsibilities of flutteractivity

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Hard

`FlutterActivity` is the native Android container that hosts a Flutter app. Its key responsibilities include:
- Bootstrapping and initializing the Flutter engine.
- Rendering the Flutter UI framework inside an Android view hierarchy.
- Handling Android platform lifecycle events (like pause, resume, back button pressed) and forwarding them to Dart.
- Managing platform channel communications.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#hard-10-list-the-responsibilities-of-flutteractivity)

---

### Hard 11. Can you describe how to implement internationalization in a flutter app

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Hard

Internationalization (i18n) is implemented in Flutter by:
1. Adding dependencies (`flutter_localizations` and `intl`) in `pubspec.yaml`.
2. Enabling the `generate: true` flag in pubspec.
3. Creating localization source files containing key-value pairs (e.g., `app_en.arb`, `app_es.arb`).
4. Declaring localizations delegates inside the main `MaterialApp` widget class.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#hard-11-can-you-describe-how-to-implement-internationalization-in-a-flutter-app)

---

### Hard 12. How do you implement a custom transition between screens in flutter

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Hard

Custom page transitions are implemented by overriding `PageRouteBuilder` instead of using standard routes. You pass a custom builder using animation parameters:

```dart
PageRouteBuilder(
  pageBuilder: (context, anim, secondaryAnim) => TargetScreen(),
  transitionsBuilder: (context, anim, secondaryAnim, child) {
    return SlideTransition(
      position: anim.drive(Tween(begin: Offset(1, 0), end: Offset.zero)),
      child: child,
    );
  },
)
```

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#hard-12-how-do-you-implement-a-custom-transition-between-screens-in-flutter)

---

### Hard 13. How do you implement a custom animation curve in flutter

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Hard

Custom animation curves are created by extending the `Curve` class and overriding the `transformInternal` method to return a calculated mathematical path value (between 0.0 and 1.0) given an input progress double:

```dart
class CustomBounceCurve extends Curve {
  @override
  double transformInternal(double t) {
    return t * t; // simple quadratic ease-in
  }
}
```

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#hard-13-how-do-you-implement-a-custom-animation-curve-in-flutter)

---

### Hard 14. Can you communicate between isolates describe an isolate

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Hard

An isolate is a separate execution thread in Dart that operates independently with its own private heap memory. Because they do not share memory space, they communicate entirely by passing messages through `SendPort` and `ReceivePort`. You can spawn a new isolate using `Isolate.spawn` or use the high-level `compute` helper function for one-off concurrent computations.

### Code Example

```dart
import 'dart:isolate';

void main() async {
  // Create a receive port to listen for messages from the isolate
  final receivePort = ReceivePort();

  // Spawn an isolate and send the receive port's sendPort to it
  await Isolate.spawn(isolateFunction, receivePort.sendPort);

  // Listen for messages from the isolate
  receivePort.listen((message) {
    print('Received message: $message');
    receivePort.close(); // Close the receive port when done
  });
}

// Function to be executed by the isolate
void isolateFunction(SendPort sendPort) {
  sendPort.send('Hello from the isolate!');
}
```

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#hard-14-can-you-communicate-between-isolates-describe-an-isolate)

---

### Hard 15. What is the flutter rendering pipeline and how does it work

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Hard

The rendering pipeline turns code into screen pixels through these phases:
1. **Build:** Widgets create and update their corresponding elements.
2. **Layout:** Render objects calculate their sizes and positions based on constraints passed down from parent elements.
3. **Paint:** Render objects generate visual painting commands.
4. **Compositing:** Visual elements are grouped into layers.
5. **Rasterization:** The engine (Impeller/Skia) converts layer commands into pixels, sending them to the GPU for presentation.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#hard-15-what-is-the-flutter-rendering-pipeline-and-how-does-it-work)

---

### Hard 16. What is the role of the flutterengine in the flutter framework

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Hard

The `FlutterEngine` is the C++ core of the framework. It handles:
- Graphics rendering (converting layer commands into GPU pixels via Skia or Impeller).
- Hosting and executing the Dart Virtual Machine (VM) and running Dart code.
- Text composition and system layout calculations.
- Handling system communication (I/O, lifecycle events, accessibility) and channel communications.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#hard-16-what-is-the-role-of-the-flutterengine-in-the-flutter-framework)

---

### Hard 17. What are platform channels in flutter and when would you use them

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Hard

Platform channels are the communication bridge between Dart and native host code (Kotlin/Java on Android, Swift/Objective-C on iOS). You use them when you need to access native API services that do not have a Flutter package, such as custom hardware integrations, battery status, or secure storage. Communication is asynchronous.

### Code Example

```dart
// Dart (Flutter)
const platform = MethodChannel('samples.flutter.dev/battery');
final batteryLevel = await platform.invokeMethod('getBatteryLevel');
```

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#hard-17-what-are-platform-channels-in-flutter-and-when-would-you-use-them)

---

### Hard 18. How do you work with multiple flutter flavors

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Hard

Flavors allow developers to build different versions of an app from a single codebase (e.g., development, staging, production). Implementing flavors involves:
1. Configuring product flavors in Android (`build.gradle`) and build schemes in iOS (Xcode).
2. Creating separate configuration entry points in Dart (e.g., `main_dev.dart`, `main_prod.dart`).
3. Running the build command specifying the target environment: `flutter run --flavor dev -t lib/main_dev.dart`.

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#hard-18-how-do-you-work-with-multiple-flutter-flavors)

---

### Hard 19. What is code splitting in flutter and how does it help

**Category:** Basics &nbsp;&nbsp;|&nbsp;&nbsp; **Difficulty:** Hard

Code splitting (deferred loading) in Flutter allows the compiler to package certain components or libraries separately, loading them on-demand at runtime rather than during app startup. This is highly useful for web applications to minimize initial download sizes. It is done using the `deferred as` import syntax:

```dart
import 'library.dart' deferred as lazyLib;

// Usage
await lazyLib.loadLibrary();
lazyLib.myFunction();
```

[Back to Index](../flutter_interview_questions.md) &nbsp;&nbsp;/&nbsp;&nbsp; [Quick Revision](../sort_questions/flutter_interview_questions_sort.md#hard-19-what-is-code-splitting-in-flutter-and-how-does-it-help)

---
