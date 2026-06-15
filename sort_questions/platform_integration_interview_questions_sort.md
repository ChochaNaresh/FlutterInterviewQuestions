# Platform Integration Interview Questions - Quick Revision

This guide contains quick-revision answers for 15 Platform Integration interview questions.

## Easy Questions

### Easy 1. What is the difference between a Flutter Package and a Flutter Plugin?

*A package is written in pure Dart and works on any system. A plugin contains both Dart wrappers and native platform code (Kotlin/Swift) to access OS-specific APIs or hardware features.*

[Back to Index](../platform_integration_interview_questions.md#easy-questions) | [Detailed Explanation](../detailed_questions/platform_integration_interview_questions.md#easy-1-what-is-the-difference-between-a-flutter-package-and-a-flutter-plugin)

### Easy 2. What is the purpose of the android/ and ios/ folders in a Flutter project structure?

*These folders contain complete, native Android (Gradle) and iOS (Xcode) projects. They act as native wrappers that host, initialize, and run the compiled Flutter engine on target devices.*

[Back to Index](../platform_integration_interview_questions.md#easy-questions) | [Detailed Explanation](../detailed_questions/platform_integration_interview_questions.md#easy-2-what-is-the-purpose-of-the-android-and-ios-folders-in-a-flutter-project-structure)

### Easy 3. What is the AndroidManifest.xml file used for on Android, and where is it located in a Flutter project?

*Located at `android/app/src/main/AndroidManifest.xml`, this file declares app permissions, native activities, entry points, and app package metadata to the Android operating system.*

[Back to Index](../platform_integration_interview_questions.md#easy-questions) | [Detailed Explanation](../detailed_questions/platform_integration_interview_questions.md#easy-3-what-is-the-androidmanifestxml-file-used-for-on-android-and-where-is-it-located-in-a-flutter-project)

### Easy 4. What is the Info.plist file used for on iOS, and where is it located in a Flutter project?

*Located at `ios/Runner/Info.plist`, this key-value XML configuration file defines iOS app settings, bundle configurations, and user-facing permission justification descriptions.*

[Back to Index](../platform_integration_interview_questions.md#easy-questions) | [Detailed Explanation](../detailed_questions/platform_integration_interview_questions.md#easy-4-what-is-the-infoplist-file-used-for-on-ios-and-where-is-it-located-in-a-flutter-project)

### Easy 5. How do you change the App Name and App Icon for both Android and iOS in Flutter?

*Change the App Name by editing `android:label` in Android's manifest and `CFBundleDisplayName` in iOS's `Info.plist`. Change App Icons easily by using the `flutter_launcher_icons` tool to generate assets.*

[Back to Index](../platform_integration_interview_questions.md#easy-questions) | [Detailed Explanation](../detailed_questions/platform_integration_interview_questions.md#easy-5-how-do-you-change-the-app-name-and-app-icon-for-both-android-and-ios-in-flutter)

## Medium Questions

### Medium 1. What is the difference between MethodChannel, EventChannel, and BasicMessageChannel?

*`MethodChannel` handles request-response patterns (one-time API actions). `EventChannel` handles native-to-Dart event streaming (sensor updates). `BasicMessageChannel` handles raw message streams.*

[Back to Index](../platform_integration_interview_questions.md#medium-questions) | [Detailed Explanation](../detailed_questions/platform_integration_interview_questions.md#medium-1-what-is-the-difference-between-methodchannel-eventchannel-and-basicmessagechannel)

### Medium 2. How does CocoaPods manage native iOS dependencies, and how do you resolve a CocoaPods version mismatch or installation issue?

*CocoaPods fetches and links native iOS libraries specified in the `Podfile`. Resolve installation blocks by running `pod deintegrate`, deleting `Podfile.lock` and the `Pods/` folder, and executing `pod install` again.*

[Back to Index](../platform_integration_interview_questions.md#medium-questions) | [Detailed Explanation](../detailed_questions/platform_integration_interview_questions.md#medium-2-how-does-cocoapods-manage-native-ios-dependencies-and-how-do-you-resolve-a-cocoapods-version-mismatch-or-installation-issue)

### Medium 3. Why do we need to customize build.gradle (module-level vs. project-level) in a Flutter application?

*The project-level `build.gradle` handles global repositories and compiler dependency versions. The module-level `build.gradle` defines build rules, target SDK versions, and signing keys.*

[Back to Index](../platform_integration_interview_questions.md#medium-questions) | [Detailed Explanation](../detailed_questions/platform_integration_interview_questions.md#medium-3-why-do-we-need-to-customize-buildgradle-module-level-vs-project-level-in-a-flutter-application)

### Medium 4. Explain how to execute platform-specific code conditionally using the Platform class or ThemeData.platform.

*Use the `Platform` class (`dart:io`) to execute different logic blocks based on the operating system. Use `Theme.of(context).platform` for widgets so that platform views can be overridden during tests.*

[Back to Index](../platform_integration_interview_questions.md#medium-questions) | [Detailed Explanation](../detailed_questions/platform_integration_interview_questions.md#medium-4-explain-how-to-execute-platform-specific-code-conditionally-using-the-platform-class-or-themedataplatform)

### Medium 5. What is the purpose of registering permissions (such as camera or location) in both AndroidManifest.xml and Info.plist?

*Registering permissions prevents security crashes at runtime. Android requires declaring permissions to unlock APIs, while iOS requires both activation and descriptive justification prompts for the user.*

[Back to Index](../platform_integration_interview_questions.md#medium-questions) | [Detailed Explanation](../detailed_questions/platform_integration_interview_questions.md#medium-5-what-is-the-purpose-of-registering-permissions-in-both-androidmanifestxml-and-infoplist)

## Hard Questions

### Hard 1. What is "Shader Compilation Jank" on iOS, and how does the Impeller rendering engine solve it compared to legacy Skia?

*Skia compiled shaders dynamically at runtime, causing frames to drop (jank) during new animations. Impeller pre-compiles shaders during build-time (AOT) and targets Metal/Vulkan directly to eliminate stutters.*

[Back to Index](../platform_integration_interview_questions.md#hard-questions) | [Detailed Explanation](../detailed_questions/platform_integration_interview_questions.md#hard-1-what-is-shader-compilation-jank-on-ios-and-how-does-the-impeller-rendering-engine-solve-it-compared-to-legacy-skia)

### Hard 2. How do you run Dart code in the background (e.g. background fetches, geofencing, or notification clicks) when the UI is closed or the app is killed?

*Run background code by annotating a callback with `@pragma('vm:entry-point')`. The OS invokes a headless Flutter engine instance, executing the callback in a separate background isolate.*

[Back to Index](../platform_integration_interview_questions.md#hard-questions) | [Detailed Explanation](../detailed_questions/platform_integration_interview_questions.md#hard-2-how-do-you-run-dart-code-in-the-background-when-the-ui-is-closed-or-the-app-is-killed)

### Hard 3. Explain how to embed a Flutter widget or screen inside an existing native Android (using FlutterActivity/FlutterFragment) or iOS (using FlutterViewController) application?

*For Add-to-App, host Flutter within a `FlutterActivity` (Android) or `FlutterViewController` (iOS). Cache the `FlutterEngine` globally in the application class to prevent loading delay.*

[Back to Index](../platform_integration_interview_questions.md#hard-questions) | [Detailed Explanation](../detailed_questions/platform_integration_interview_questions.md#hard-3-explain-how-to-embed-a-flutter-widget-or-screen-inside-an-existing-native-android-or-ios-application)

### Hard 4. How does ProGuard / R8 work for Android obfuscation and size reduction, and how do you configure it in a Flutter project?

*R8 performs code shrinking and obfuscation to optimize app size and security. Configure it by setting `minifyEnabled true` in `build.gradle` and defining keep-rules in `proguard-rules.pro`.*

[Back to Index](../platform_integration_interview_questions.md#hard-questions) | [Detailed Explanation](../detailed_questions/platform_integration_interview_questions.md#hard-4-how-does-proguard-r8-work-for-android-obfuscation-and-size-reduction-and-how-do-you-configure-it-in-a-flutter-project)

### Hard 5. How does Flutter handle iOS App Signing and Provisioning Profiles, and what is the difference between Development, Ad-Hoc, and App Store distribution profiles?

*Apple signing requires developer certificates and provisioning profiles. Development and Ad-Hoc profiles restrict execution to registered device UUIDs, while App Store profiles authorize global public release.*

[Back to Index](../platform_integration_interview_questions.md#hard-questions) | [Detailed Explanation](../detailed_questions/platform_integration_interview_questions.md#hard-5-how-does-flutter-handle-ios-app-signing-and-provisioning-profiles-and-what-is-the-difference-between-development-ad-hoc-and-app-store-distribution-profiles)
