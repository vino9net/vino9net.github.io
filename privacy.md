# Sightly AI Privacy Policy

_Last updated: 2026-04-24_

Sightly AI ("the app") is a tourist-aid application that uses the camera,
microphone, and location sensors on your device to help you understand the
places around you — museums, historical sites, churches, restaurants, and
street scenes — and to translate menus and signs. This document describes
what data the app collects, how it is used, and which third-party services
receive it.

## Who operates the app

The app is developed and operated by an independent developer. For
privacy questions or data-deletion requests, contact:
**guru.lin@gmail.com**.

## What the app collects and why

- **Location (latitude, longitude).** Collected via Google Play Services
  (FusedLocationProvider) only while the app is in the foreground and
  only when you take a photo. Used to find nearby points of interest.
  Never written to permanent storage on our servers.
- **Camera frames.** The image you capture is processed on-device by
  Google's Gemini Nano model (via Android ML Kit GenAI) to classify the
  scene. A compressed version may be sent to Google's Gemini Flash/Pro
  model (via Firebase AI Logic) for deeper answers you explicitly
  request. Photos are not retained after the request completes.
- **Microphone audio.** Captured only when you activate voice chat.
  Processed by the same Gemini models as camera frames. Not retained.
- **Anonymous account identifier.** Firebase Authentication issues a
  randomly generated anonymous user ID on first launch, used to apply
  per-user rate limits and to scope any saved preferences. It is not
  linked to your name, email, or device identifier.
- **Crash and diagnostic data.** Firebase Crashlytics collects stack
  traces, device model, OS version, and app version when the app
  crashes, so we can fix bugs. No user content is included.
- **Push notification token.** Firebase Cloud Messaging issues a device
  token used only to deliver in-app notifications you have opted into.

The app does **not** collect your name, phone number, email address,
contacts, photo library, SMS, call log, or advertising ID.

## Third-party services

The app shares the minimum data required with the following services.
Each has its own privacy policy that also governs your data.

- **AMAP (高德地图)** — when your device is in mainland China, the app
  sends your current latitude and longitude to AMAP's POI search API
  to find nearby places. See
  <https://lbs.amap.com/pages/privacy/>.
- **Google Places API** — outside mainland China, the same latitude
  and longitude is sent to Google Places instead. See
  <https://policies.google.com/privacy>.
- **Firebase (Google)** — used for anonymous authentication,
  crash reporting, push messaging, and cloud AI inference. See
  <https://firebase.google.com/support/privacy>.
- **Google ML Kit / Gemini Nano** — runs entirely on your device; no
  data leaves the device for this path.

## Data retention

- Location coordinates are used in-memory for the duration of one POI
  lookup and then discarded.
- Camera and microphone content is used in-memory for the duration of
  one analysis and then discarded.
- Crashlytics diagnostic records are retained by Google for up to 90
  days, per Firebase defaults.

## Your rights

You may at any time:

- Revoke camera, microphone, or location permission from Android
  Settings. The corresponding features will stop working but the app
  will continue to run.
- Uninstall the app to delete its local preferences and the anonymous
  user ID.
- Email **guru.lin@gmail.com** to request deletion of any data
  associated with your anonymous user ID.

## Children

The app is not directed at children under 13. We do not knowingly
collect data from children under 13.

## Changes to this policy

Material changes will be announced in-app and reflected in the
"Last updated" date above.
