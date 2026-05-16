# Grama-Angana

Grama-Angana is a community space management Android app for village halls (Angana / Samudaya Bhavana) built with modern Android architecture.

## Tech Stack
- Kotlin
- MVVM + Clean Architecture
- Jetpack Compose + Material 3
- Hilt Dependency Injection
- Firebase Authentication + Firestore + FCM
- Room Database for offline cache
- Coroutines + StateFlow
- Navigation Compose
- Coil (image loading)
- Lottie Compose (motion animations)

## Modern UI Screens (Demo-Ready)
1. Splash screen with animated entry
2. Premium login/register screen
3. Home dashboard with banner/stats/feature cards
4. Hall availability calendar (green/red/yellow states)
5. Booking request form screen with snackbar feedback
6. Events feed with image cards
7. Maintenance hub progress cards
8. My requests tracker screen
9. Profile screen

## Folder Architecture
`app/src/main/java/com/grama/angana`
- `data/local` Room entities, DAO, DB
- `data/repository` Firebase + local data sources
- `domain/model` business models
- `domain/repository` repository contracts
- `di` Hilt modules
- `presentation/auth` auth UI + ViewModel
- `presentation/navigation` splash + bottom-nav + all UI screens
- `ui/theme` colors and app theme

## Bottom Navigation
- Home
- Calendar
- Events
- Requests
- Profile

## Firestore Collections
- `users`
- `bookings`
- `events`
- `maintenance_items`
- `contributions`

## Setup Instructions
1. Open in Android Studio.
2. Sync Gradle.
3. Create Firebase project and Android app package `com.grama.angana`.
4. Add `google-services.json` inside `app/`.
5. Enable Email/Password auth and Phone auth.
6. Create Firestore database and apply `firebase.rules`.
7. Build and run on Android 8.0+ device.

## Dummy Data Seeds (Firestore)
Use these documents after creating collections:
- `events/demo_event_1`: title `Health Camp`, date `2026-05-15`
- `maintenance_items/bulbs`: targetAmount `5000`, collectedAmount `1600`, supporters `12`
- `bookings/demo_booking_1`: status `PENDING`, date `2026-05-20`, timeSlot `10:00-12:00`

## Next Steps for Full Production
- Add phone OTP verification UI and backend checks.
- Implement Firestore transactions for strict duplicate slot prevention.
- Add admin moderation workflows and analytics charts.
- Add push notification triggers for approval/rejection.
- Add search/filter/history/profile screens.
