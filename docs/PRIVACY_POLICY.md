# Pulse Privacy Policy

Last updated: 2026-09-03

Pulse is designed to be local-first. It does not require an account, does not use a server, does not include ads, and does not use third-party analytics.

## Health Data

With your permission, Pulse may read the following data from Apple Health:

- Heart rate.
- Blood oxygen.
- Step count.
- Active energy burned.
- Resting energy burned (`basalEnergyBurned` in HealthKit).
- Workout intervals.
- Sleep intervals and sleep stages.

Pulse uses this data in the relevant app surfaces. Active and resting energy are used to show calories burned today on the iPhone Home screen and calorie history in History. Other supported readings may also appear in widgets, Apple Watch views, and Apple Watch complications.

Pulse may also use these readings on device to calculate factual daily context, such as a step-pace comparison with the user's own previous days, sleep summaries, monthly History buckets, and consistency progress. Pulse does not use these calculations to diagnose a condition, determine medical risk, or create a medical or readiness score.

## Local Storage

Pulse stores compact, versioned local snapshots on your devices so the app, widgets, and Apple Watch surfaces can show the latest known values and truthful trends quickly. A snapshot can include values, units, measured timestamps, freshness state, a bounded set of timestamped trend points, and display preferences. Widget snapshots stay in the app-group container. Data sent between the user's iPhone and Apple Watch stays within Apple's device-to-device services and is not sent to Pulse or the developer.

Depending on the features you use, other app-owned local state can include display, onboarding, and appearance preferences; your Consistency enrollment day, selected companion, program-timezone and step-goal revisions, and credited active-day keys; earned achievements and pending reward presentation state; notification preferences and bounded scheduling records; and the current Step Quest Live Activity identifier and limited progress state.

Credited Consistency days and earned badges are local achievement records. Deleting samples from Apple Health does not automatically remove those earned records. Reset Consistency Progress removes the local Consistency program state without deleting or changing Apple Health data.

Workout and sleep data are read from Apple Health for chart context and summaries. Pulse does not create a separate cloud health database.

Active and resting energy are read from Apple Health when Pulse refreshes the calorie views. Pulse derives total calories on device by adding the two components when both are available. Pulse does not maintain a separate raw calorie database or persist a standalone total-calorie record.

Pulse stores notification preferences and sanitized local scheduling diagnostics so it can reconcile reminders and explain failures. Scheduling records are retained for at most 90 days. Pulse may also keep local counters for days of use, successful refreshes, Brief views or taps, notification taps, and use of the Year range. These counters contain no Health values, notification bodies, attachments, or personal identifiers. They are used only for on-device eligibility and a local debug report and are never transmitted.

## Local Notifications and Lock Screen Privacy

Pulse uses local notifications only. It does not use a remote notification server.

Notification permission and Daily Check-in are separate choices. When both are enabled, a recent on-device Apple Health update may replace the generic check-in with a concise summary containing available Health values such as steps, calories, sleep, heart rate, or blood oxygen. Pulse applies metric-specific freshness limits and falls back to generic text when data is missing or old.

Health values may therefore appear on the Lock Screen, in Notification Center, or on a paired Apple Watch. Apple controls notification previews, Lock Screen visibility, Focus, Scheduled Summary, sound, and delivery behavior. Users can hide previews or disable Pulse notifications at any time in iOS Settings. Disabling reminders stops future Pulse scheduling without transmitting or deleting Health data.

## Step Quest and Live Activities

Step Quest is a Live Activity started explicitly by the user. Its content is computed locally from the current step total and goal. Pulse stores only the current activity identifier and limited progress state while it is running. Step Quest does not start automatically in the background, does not send progress to a Pulse server, and does not save a workout or other sample to Apple Health.

## Data Collection

Pulse does not transmit your health data to the developer, a server, advertisers, analytics providers, or data brokers.

Pulse does not collect health data for advertising, marketing, tracking, profiling, or data mining.

The app's privacy manifests declare no collected data and no tracking. They declare only the required-reason API access used for local and app-group preferences.

Apple may process HealthKit, notification, Live Activity, iCloud, device, or App Store information under Apple's own terms and privacy policies. Pulse does not control Apple's platform processing.

Under Apple's App Privacy definitions, Pulse's disclosure is `Data Not Collected` because Health data, preferences, snapshots, and sanitized counters are processed on the user's devices and are not transmitted to the developer or third parties. This disclosure must be revisited before adding any server, analytics, crash-reporting SDK, remote notification provider, support form, cloud sync, or external telemetry.

## Voluntary Support Communication

The Pulse app does not transmit support messages. If you voluntarily contact support through GitHub Issues or email, GitHub or your email provider processes the information you choose to provide under its own terms. The developer uses that information only to respond to the request and does not combine it with Apple Health data. Do not include Health values, medical information, personal identifiers, or sensitive screenshots in a support request.

Support correspondence is retained only as reasonably necessary to respond, maintain an accurate issue history, or meet legal obligations. You can delete your own GitHub content where GitHub permits it or request deletion of support correspondence using the contact below. This voluntary communication occurs outside the app and does not change Pulse's App Store privacy disclosure for data collected from the app.

## Apple Watch Sensor Checks

Pulse can start a short Apple Watch heart-rate sensor check. Apple requires a HealthKit workout-session API path for near-live heart-rate access on Apple Watch. Pulse discards that session and does not save a workout to Apple Health or Fitness history.

Blood oxygen is shown only as the latest available Apple Health sample. Pulse does not provide live blood oxygen monitoring.

## Permissions

You can grant or revoke Health permissions at any time in the Apple Health app or iOS Settings.

You can grant, limit, or revoke notification permission in iOS Settings. Inside Pulse, the notification master switch, Daily Check-in, Gentle Return, and Live Activity preferences remain separate controls. Turning off the master suspends Pulse notification activity without silently enabling or changing the child preferences.

## Retention and Deletion

Apple Health remains the source of truth. Revoking Pulse's Health access stops future reads but does not delete the user's records from Apple Health. Resetting Consistency removes only Pulse's local program state and leaves Apple Health unchanged. Removing Pulse and its extensions removes app-owned local snapshots, preferences, diagnostics, and counters according to iOS app-container behavior; it does not delete Apple Health records.

## Medical Disclaimer

Pulse is for personal glanceable tracking only. It is not a medical device and is not intended to diagnose, treat, cure, monitor, or prevent any disease or medical condition. Always consult a qualified healthcare professional for medical questions.

## Contact

For product support, bug reports, general feedback, and feature requests, use the public [Pulse Support page](https://github.com/roccodaffuso/Pulse/blob/main/SUPPORT.md). For private questions or if you cannot use GitHub Issues, contact Rocco D'Affuso at [roccodaffuso@gmail.com](mailto:roccodaffuso@gmail.com).
