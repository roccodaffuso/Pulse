# Pulse Privacy Policy

Last updated: 2026-08-03

Pulse is designed to be local-first. It does not require an account, does not
use a developer-operated backend, does not include advertising, and does not
use third-party analytics or tracking SDKs.

## Health Data

With your permission, Pulse may read the following data from Apple Health:

- Heart rate.
- Blood oxygen.
- Step count.
- Workout intervals.
- Sleep intervals and sleep stages.

Pulse uses this data to present your latest vitals, factual history and sleep
summaries, consistency progress, widgets, Apple Watch views, and Apple Watch
complications. HealthKit remains the source of truth for health samples. Pulse
does not create a separate cloud health database.

## Local Storage

Pulse stores only the local information needed to operate its app, widgets,
Apple Watch surfaces, reminders, and consistency program. Depending on the
features you use, this can include:

- A compact snapshot of the latest known metrics, units, measurement times,
  availability, and freshness.
- Display, onboarding, and appearance preferences.
- Your consistency enrollment day, selected companion, program-timezone
  revisions, step-goal revisions, and credited active-day keys.
- Earned achievements, badges already presented, and pending local reward
  presentation state.
- Notification preferences and bounded delivery markers used to avoid
  duplicate reminders.
- The current local Step Quest Live Activity identifier and its limited
  progress state while the activity is running.
- Technical refresh metadata in local Debug builds only. Debug reports exclude
  heart-rate, blood-oxygen, and step-count values and are never uploaded
  automatically.

Some compact snapshots and display preferences are stored in an Apple app
group so the iPhone app, widgets, Apple Watch app, and complications can render
consistently. Pulse does not duplicate full raw HealthKit history when it can
query Apple Health on demand.

Credited consistency days and earned badges are local achievement records.
Deleting samples from Apple Health does not automatically remove those earned
records. `Reset Consistency Progress` in Pulse removes the local consistency
program state without deleting or changing Apple Health data.

## Notifications And Live Activities

Pulse notifications are local and opt-in. Notification authorization is
requested only after you enable reminders in Settings. Pulse currently uses
local daily-progress and gentle-return reminders; it does not use remote push
notifications.

Step Quest is a Live Activity started explicitly by the user. Its content is
computed locally from the current step total and goal. It does not start
automatically in the background and does not send progress to a Pulse server.

## Apple Watch Sensor Checks

Pulse can start a short Apple Watch heart-rate sensor check. Apple requires a
HealthKit workout-session API path for near-live heart-rate access on Apple
Watch. Pulse discards that session and does not save a workout to Apple Health
or Fitness history.

Blood oxygen is shown only as the latest available Apple Health sample. Pulse
does not provide live blood-oxygen monitoring.

## Data Collection And Sharing

Pulse does not transmit health data or consistency data to the developer, a
server, advertisers, analytics providers, or data brokers. It does not collect
data for advertising, marketing, tracking, profiling, or data mining.

The app's privacy manifests declare no collected data and no tracking. They
declare only the required-reason API access used for local and app-group
preferences.

Apple may process HealthKit, notification, Live Activity, iCloud, device, or
App Store information under Apple's own terms and privacy policies. Pulse does
not control Apple's platform processing.

## Permissions And Control

You can grant or revoke Health permissions at any time in the Apple Health app
or iOS Settings. You can disable Pulse reminders and Live Activities from
Pulse Settings. Removing the app removes its app-local data subject to Apple's
normal device and backup behavior.

## Medical Disclaimer

Pulse is for personal glanceable tracking only. It is not a medical device and
is not intended to diagnose, treat, cure, monitor, or prevent any disease or
medical condition. Always consult a qualified healthcare professional for
medical questions.

## Contact

For privacy questions or support, use
[Pulse Support](https://github.com/roccodaffuso/Pulse/issues).
