# FirebaseNotification
This respository is a simple project for Firebase Notification on iOS application.  
 1) Include pod 'Firebase/Messaging'
 2) Configure APNs Certificates following this step below...
    - 2.1) Create a certificate signing request ==> Open “Keychain Access” → Certificate Assistant → Request a Certificate From a Certificate Authority → Enter email address → Check “Saved to disk” → Continue → Specify a location & click “Save”
    - 2.2) Download development certificate ==> Go to developer.apple.com → Certificates, Identifiers & Profiles → Identifiers → “your app” → Push Notification → Create Certificate → Choose File (choose the development certificate) → Download
    - 2.3) Export .p12 file ==> click the certificate that you downloaded, then go to “Keychain Access” → select “my certificates” → find the certificate → right click → “export” → “save”
    - 2.4) Upload certificate to Firebase ==> Open Firebase, and go to Project Settings → Cloud Messaging → APNS Certificates → upload the certificate
 3) Set up app with push notification on capability and swift code on AppDelegate file

## How to fix bug on testFlight
- Import another certifacation on firebase for production enviroment 
- https://stackoverflow.com/questions/41140631/firebase-push-notifications-not-working-on-testflight-adhoc-release
- https://stackoverflow.com/questions/47022963/firebase-notifications-issue-with-ios-in-testflight
- https://stackoverflow.com/questions/24044298/why-push-notifications-is-not-working-on-testflight

## Source
- https://medium.com/plus-minus-one/configure-firebase-push-notification-f0e9f035c81b
- https://firebase.google.com/docs/cloud-messaging/ios/client#swift
- https://www.youtube.com/watch?v=pVtIVfJJ35w
- https://www.raywenderlich.com/20201639-firebase-cloud-messaging-for-ios-push-notifications

### Test Project by Lee McCormick
Learning Switf and Xcode is my passion. This project was built by following the tutorial and source code online.
