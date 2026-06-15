# App Deployment & Notifications Interview Questions - Quick Revision

This guide contains quick-revision answers for 12 App Deployment & Notifications interview questions.

## Easy Questions

### Easy 1. What is the difference between an APK, an App Bundle (AAB), and an IPA file?

*An APK is a ready-to-install Android file. An AAB is Google Play's publishing format that generates smaller, device-optimized APKs dynamically. An IPA is the standard compiled binary package for iOS apps.*

[Back to Index](../app_deployment_and_notifications_questions.md#easy-questions) | [Detailed Explanation](../detailed_questions/app_deployment_and_notifications_questions.md#easy-1-what-is-the-difference-between-an-apk-an-app-bundle-aab-and-an-ipa-file)

### Easy 2. What is FCM (Firebase Cloud Messaging) and why is it commonly used in Flutter apps?

*FCM is Google's cross-platform push service. It acts as a unified bridge to route messages to both Android and iOS devices, simplifying server push configurations.*

[Back to Index](../app_deployment_and_notifications_questions.md#easy-questions) | [Detailed Explanation](../detailed_questions/app_deployment_and_notifications_questions.md#easy-2-what-is-fcm-firebase-cloud-messaging-and-why-is-it-commonly-used-in-flutter-apps)

### Easy 3. What is TestFlight on iOS and Internal Testing on Android?

*TestFlight (iOS) and Internal Testing (Android) are beta distribution tracks that allow you to distribute pre-release builds to select testers instantly, bypassing standard App Store review delays.*

[Back to Index](../app_deployment_and_notifications_questions.md#easy-questions) | [Detailed Explanation](../detailed_questions/app_deployment_and_notifications_questions.md#easy-3-what-is-testflight-on-ios-and-internal-testing-on-android)

### Easy 4. What are APNs (Apple Push Notification service) and how do they differ from FCM?

*APNs is Apple's native notification router for iOS. While FCM is cross-platform, FCM must route its iOS notification requests through APNs to reach Apple devices.*

[Back to Index](../app_deployment_and_notifications_questions.md#easy-questions) | [Detailed Explanation](../detailed_questions/app_deployment_and_notifications_questions.md#easy-4-what-are-apns-apple-push-notification-service-and-how-do-they-differ-from-fcm)

## Medium Questions

### Medium 1. Explain the difference between Foreground, Background, and Terminated states when handling push notifications in Flutter.

*In the foreground, notifications trigger a Dart callback without a system banner. In the background, the OS displays a banner, triggering a callback on click. In the terminated state, you read the launching payload via `getInitialMessage()`.*

[Back to Index](../app_deployment_and_notifications_questions.md#medium-questions) | [Detailed Explanation](../detailed_questions/app_deployment_and_notifications_questions.md#medium-1-explain-the-difference-between-foreground-background-and-terminated-states-when-handling-push-notifications-in-flutter)

### Medium 2. How do you configure push notifications for iOS (including APNS certificates, .p8 keys, and Provisioning Profiles)?

*Enable Push capabilities in Xcode, generate a `.p8` APNs auth key in the Apple Developer console, upload it to your push server (Firebase), and ensure your provisioning profile contains push entitlements.*

[Back to Index](../app_deployment_and_notifications_questions.md#medium-questions) | [Detailed Explanation](../detailed_questions/app_deployment_and_notifications_questions.md#medium-2-how-do-you-configure-push-notifications-for-ios)

### Medium 3. What is Fastlane and how is it used to automate Flutter app publishing?

*Fastlane automates mobile app deployment. Operating inside the native directories, it uses scripts (Fastfiles) to automate code signing, compile binaries, and upload releases directly to TestFlight and Google Play.*

[Back to Index](../app_deployment_and_notifications_questions.md#medium-questions) | [Detailed Explanation](../detailed_questions/app_deployment_and_notifications_questions.md#medium-3-what-is-fastlane-and-how-is-it-used-to-automate-flutter-app-publishing)

### Medium 4. How do you request and handle user notification permissions dynamically in Flutter?

*Request permissions using `FirebaseMessaging.instance.requestPermission()`. Check the returned status dynamically to either proceed with push registration or guide users to system settings if denied.*

[Back to Index](../app_deployment_and_notifications_questions.md#medium-questions) | [Detailed Explanation](../detailed_questions/app_deployment_and_notifications_questions.md#medium-4-how-do-you-request-and-handle-user-notification-permissions-dynamically-in-flutter)

## Hard Questions

### Hard 1. Explain how to handle notification payload clicks to deep-link users to a specific screen when the app is opened from a terminated state.

*Include data tags (like `{route: '/page'}`) inside the push payload. Read these values during app boot using `FirebaseMessaging.instance.getInitialMessage()`, routing users to the target screen once layout initializes.*

[Back to Index](../app_deployment_and_notifications_questions.md#hard-questions) | [Detailed Explanation](../detailed_questions/app_deployment_and_notifications_questions.md#hard-1-explain-how-to-handle-notification-payload-clicks-to-deep-link-users-to-a-specific-screen-when-the-app-is-opened-from-a-terminated-state)

### Hard 2. How do you set up a Continuous Integration / Continuous Deployment (CI/CD) pipeline for a Flutter app (e.g. using GitHub Actions or Codemagic)?

*Automate testing, build compiles, code signing, and binary uploads using CI workflows. Securely inject signing keys and profiles via pipeline variables to generate production AAB/IPA files.*

[Back to Index](../app_deployment_and_notifications_questions.md#hard-questions) | [Detailed Explanation](../detailed_questions/app_deployment_and_notifications_questions.md#hard-2-how-do-you-set-up-a-continuous-integration-continuous-deployment-cicd-pipeline-for-a-flutter-app)

### Hard 3. What are Notification Service Extensions on iOS, and how do you implement them in a Flutter project to show rich notifications (with images or media)?

*Create a native iOS Notification Service Extension target in Xcode. It intercepts notifications containing `mutable-content: 1` in the payload to download and attach rich media before displaying the banner.*

[Back to Index](../app_deployment_and_notifications_questions.md#hard-questions) | [Detailed Explanation](../detailed_questions/app_deployment_and_notifications_questions.md#hard-3-what-are-notification-service-extensions-on-ios-and-how-do-you-implement-them-in-a-flutter-project-to-show-rich-notifications)

### Hard 4. How do you manage push notification tokens (token refreshing, storing on backend, and cleaning up expired tokens)?

*Fetch the token on boot and update it by listening to `onTokenRefresh`. On the backend, delete tokens during user logout and automatically purge stale tokens when notification gateways return delivery failure errors.*

[Back to Index](../app_deployment_and_notifications_questions.md#hard-questions) | [Detailed Explanation](../detailed_questions/app_deployment_and_notifications_questions.md#hard-4-how-do-you-manage-push-notification-tokens)
