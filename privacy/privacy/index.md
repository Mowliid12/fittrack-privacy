# FitTrack Privacy Policy

**Effective date:** October 3, 2026
**Last updated:** October 3, 2026

## 1. Introduction

This Privacy Policy explains how FitTrack ("FitTrack," "the app," "we," "us") collects, uses, stores, and protects information when you use the FitTrack mobile application. FitTrack is developed and published by Zahid Labs ("Zahid Labs," "we," "our").

FitTrack is a personal fitness and body-transformation tracking app that helps you follow workouts, log body measurements, track nutrition, save progress photos, and set reminders. This policy describes what information the app actually collects and how it is handled, based on the app's current functionality.

By using FitTrack, you agree to the collection and use of information as described in this policy. If you do not agree, please do not use the app.

## 2. Information We Collect

FitTrack collects the following categories of information:

- **Account and identity information** — such as your email address, name, and authentication details, managed through our authentication provider, Clerk.
- **Profile and fitness information** — such as your age, sex, height, activity level, fitness goal, tracking preferences, unit preferences, and workout settings.
- **Body progress data** — such as weight, body fat percentage, and body measurements (chest, waist, hips, neck, arms, thighs) that you choose to log.
- **Workout data** — such as workout sessions, exercises performed, sets, reps, duration, and timestamps.
- **Nutrition data** — such as nutrition goals, logged food entries (selected from our food catalog), portions, meal type, calories, and macronutrients, along with the date and time each entry was logged.
- **User content** — such as progress photos and an optional custom profile photo that you choose to upload.
- **Reminder preferences** — such as which reminders you enable and the times/days you choose for them.
- **Device-local information** — such as your authentication session, an in-progress onboarding draft, and local notification scheduling data, stored securely on your device.

We only collect information that you actively provide by using the app's features. We do not require you to fill in every field — many fields described above are optional, and the app is designed to show an honest empty state rather than fabricated data when something has not been entered.

## 3. How We Use Information

We use the information described above to:

- Create and manage your account and keep you signed in.
- Provide the app's core features — tracking your workouts, measurements, nutrition, and progress photos, and showing you your own data and progress over time.
- Personalize your experience based on the goals and preferences you provide.
- Schedule and deliver local reminder notifications that you choose to enable.
- Maintain the security and integrity of the app, including verifying that you are the owner of the data you are accessing.
- Allow you to edit or delete your data and, if you choose, delete your account.

We do not use your information for advertising, and we do not sell your personal information.

## 4. Authentication and Account Services

FitTrack uses **Clerk** to manage authentication and account identity. Depending on how you choose to sign in, Clerk may process information such as your email address, name/profile information, and authentication or session information.

FitTrack supports the following sign-in methods:

- **Email and password.** Clerk manages your password directly. FitTrack's own database (provided by Convex) does **not** store your password or any authentication secret.
- **Google Sign-In.**
- **Apple Sign-In**, where offered on supported iOS configurations.

When you sign in with Google or Apple, authentication is brokered through Clerk. FitTrack's own code does not receive or store your Google or Apple password or raw credentials — only a resulting authenticated session.

To connect your authentication identity to your FitTrack data, our database stores a reference to your Clerk user ID. It does not separately store your email address or name as a duplicate copy — your profile display information continues to be managed through Clerk.

## 5. Fitness, Body Measurement and Nutrition Data

To provide FitTrack's core functionality, we store the fitness and health-related information you provide, including:

- Profile and goal information: age, sex, height, activity level, fitness goal, tracking preferences, unit preferences, and workout settings.
- Body progress data: weight, body fat percentage, and any body measurements you log (chest, waist, hips, neck, arms, thighs).
- Workout history: workout sessions you start or complete, the exercises and sets/reps involved, session duration, and timestamps.
- Nutrition data: your nutrition goals and food entries you log (selected from FitTrack's built-in food catalog), including portion size, meal type, calories, and macronutrients, along with when each entry was logged.

This information is used solely to power the app's tracking and progress features for your own account. It is not used for advertising and is not sold.

## 6. Photos and User Content

FitTrack lets you optionally save progress photos and an optional custom profile photo. These images are stored using our database provider's (Convex) secure file storage system, along with basic metadata such as the photo type and the date it was taken.

Before the app ever shows you a photo or provides a link to one, it verifies that you are the account that owns it — the app does not let one account browse or retrieve another account's photos.

We want to describe this accurately: like many cloud file-storage systems, the direct link used to display a stored photo is not itself re-checked against your login every single time it is loaded. FitTrack never shares, publishes, or exposes these links to anyone else, and the app only ever hands a photo's link to the account that owns it. However, we cannot guarantee absolute confidentiality of a link if it were somehow independently obtained and shared outside of the app by a third party. You remain in control of your photos and can delete them at any time (see Section 12).

## 7. Notifications and Device Permissions

FitTrack currently uses **local, on-device notifications** for reminders (for example, workout, nutrition, measurement, or progress-photo reminders) that you can enable, configure, and disable. These reminders are scheduled directly on your device using your device's local time.

- FitTrack does **not** currently generate or use a push-notification token, and does **not** currently use any remote/server-sent push notification service.
- Your reminder preferences (such as enabled status, time, and recurrence) are stored in our database so they can be restored if you reinstall the app or sign in on another device. The underlying on-device schedule identifiers are kept only on your device.

FitTrack requests the following device permissions, each used only for the specific feature described:

- **Camera** — to let you take a progress photo or a profile photo directly within the app.
- **Photo Library** — to let you select an existing photo for a progress photo or profile photo.
- **Notifications** — to deliver the local reminders described above. We only request this permission when you choose to enable a reminder, not automatically on launch.
- **Internet/network access** — required for the app to communicate with our authentication and database providers.

FitTrack does not use your device's microphone for any feature, and does not request microphone access.

## 8. How Information Is Stored

FitTrack relies on the following storage locations:

- **Clerk** stores your authentication and account identity information (such as email, password, and session data).
- **Convex**, our database and file-storage provider, stores your FitTrack app data — profile and fitness information, body measurements, workout history, nutrition entries, reminder preferences, and your uploaded photos.
- **Your device**, using secure, encrypted local storage, keeps your authentication session, an in-progress onboarding draft (if you haven't finished setting up your profile yet), and local notification scheduling information. This device-local information is not a substitute for, or separate copy of, your account — it supports the app's day-to-day operation on your device.

## 9. Service Providers

FitTrack relies on the following service providers to operate:

| Provider | Role |
|---|---|
| **Clerk** | Authentication, account identity, session management, and brokering Google/Apple sign-in. |
| **Convex** | Backend database and file storage for your FitTrack app data. |
| **Google** | Provides optional Google Sign-In authentication, if you choose to use it. |
| **Apple** | Provides optional Apple Sign-In authentication on supported iOS configurations, if you choose to use it. |
| **Expo** | Provides the application/runtime infrastructure the app is built on, including the local notification scheduling APIs described in Section 7. |

These providers may process information according to their own terms of service and privacy documentation, in their role of helping us provide the FitTrack service. We do not permit these providers to use your FitTrack data for their own advertising purposes, and none of them are used by FitTrack for advertising.

## 10. Analytics, Advertising and Tracking

As of the date of this policy, FitTrack does not include:

- Any advertising SDK or behavioral advertising.
- Any analytics or usage-tracking SDK.
- Any crash-reporting SDK.
- Any attribution/marketing-tracking SDK.
- Location or GPS tracking.
- Cookies or similar technology used for behavioral tracking.

We do not sell your personal information.

This section describes our current practice as implemented in the app. If this were to change in a future version of the app, this policy would be updated accordingly before such a change takes effect.

## 11. Data Retention

FitTrack does not currently apply an automatic data-retention timer or automatic deletion schedule to your app data. Your information is retained until:

- You delete an individual supported record (for example, a specific body measurement or a nutrition entry), where the app supports doing so; or
- You delete your FitTrack account (see Section 12).

Our service providers (such as Clerk and Convex) may retain limited information for a short additional period where required for legal, security, fraud-prevention, or backup purposes, in accordance with their own policies. We do not promise instantaneous removal from every backup system at every provider.

## 12. Account and Data Deletion

You can request deletion of your account directly within the app (Profile → Settings → Delete Account). When you do, FitTrack removes your account-owned data from our database, including:

- Your profile, fitness goal, and preference information.
- Your body measurements.
- Your workout session history.
- Your nutrition goals and logged food entries.
- Your progress photo records and the associated stored photo files.
- Your reminder preferences.
- Your local on-device notification scheduling state and onboarding draft.

Your authentication account with Clerk is also deleted as part of this process. Account deletion is permanent and cannot be undone through the app.

As noted in Section 11, our service providers may retain limited information for a short period where their own legal, security, or backup obligations require it.

## 13. Data Security

We take reasonable, practical steps to protect your information, including:

- Requiring authentication to access your account and data.
- Verifying ownership of a record before it is shown, edited, or deleted — your data is scoped to your own account.
- Storing your authentication session and other sensitive on-device information using your device's secure, encrypted storage.

No method of electronic storage or transmission is completely secure. While we work to protect your information using practices like those above, we cannot guarantee absolute security, and we do not claim that your information is "100% secure" or impossible to access under any circumstance.

## 14. International Data Processing

FitTrack's service providers may process and store information in countries other than the one you live in. Where this occurs, those providers are responsible for handling information in accordance with their own applicable privacy and data-protection obligations.

## 15. Your Privacy Rights

Within the app, you can:

- Access and view your own app data.
- Edit supported profile, goal, and measurement information.
- Delete supported individual entries (such as a measurement or a nutrition entry).
- Delete your account and associated FitTrack data, as described in Section 12.

Depending on where you live, you may have additional rights regarding your personal information under applicable law (for example, rights available to residents of the EEA/UK under GDPR, or to California residents under applicable state law). These rights, and how to exercise them, can vary by jurisdiction — not every right described in general privacy regulations is guaranteed to be identical in every country or region. If you would like to exercise a privacy right not already available directly in the app, please contact us using the information in Section 18.

## 16. Children's Privacy

FitTrack V1 is intended for users aged 18 and older. Users under 18 are not permitted to use FitTrack.

FitTrack does not knowingly intend to collect personal information from users under 18. If Zahid Labs becomes aware that information from a user under 18 has been collected, appropriate steps may be taken to delete it.

If you believe a user under 18 has provided us with personal information, please contact us using the information in Section 18 so we can take appropriate action.

## 17. Changes to This Privacy Policy

We may update this Privacy Policy from time to time, including as FitTrack's features change. If we make material changes, we will update the "Last updated" date at the top of this policy. We encourage you to review this policy periodically.

## 18. Contact Us

If you have questions about this Privacy Policy or how FitTrack handles your information, please contact:

**Zahid Labs**
Email: zahidlabs.support@gmail.com
