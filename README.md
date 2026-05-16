Grama-Angana

Grama-Angana is a community space management Android app for village halls (Angana / Samudaya Bhavana) built with modern Android architecture.

Tech Stack
Kotlin
MVVM + Clean Architecture
Jetpack Compose + Material 3
Hilt Dependency Injection
Firebase Authentication + Firestore + FCM
Room Database for offline cache
Coroutines + StateFlow
Navigation Compose
Coil (image loading)
Lottie Compose (motion animations)
Modern UI Screens (Demo-Ready)
Splash screen with animated entry
Premium login/register screen
Home dashboard with banner/stats/feature cards
Hall availability calendar (green/red/yellow states)
Booking request form screen with snackbar feedback
Events feed with image cards
Maintenance hub progress cards
My requests tracker screen
Profile screen
Folder Architecture

app/src/main/java/com/grama/angana

data/local Room entities, DAO, DB
data/repository Firebase + local data sources
domain/model business models
domain/repository repository contracts
di Hilt modules
presentation/auth auth UI + ViewModel
presentation/navigation splash + bottom-nav + all UI screens
ui/theme colors and app theme
Bottom Navigation
Home
Calendar
Events
Requests
Profile
Firestore Collections
users
bookings
events
maintenance_items
contributions
Setup Instructions
Open in Android Studio.
Sync Gradle.
Create Firebase project and Android app package com.grama.angana.
Add google-services.json inside app/.
Enable Email/Password auth and Phone auth.
Create Firestore database and apply firebase.rules.
Build and run on Android 8.0+ device.
Dummy Data Seeds (Firestore)

Use these documents after creating collections:

events/demo_event_1: title Health Camp, date 2026-05-15
maintenance_items/bulbs: targetAmount 5000, collectedAmount 1600, supporters 12
bookings/demo_booking_1: status PENDING, date 2026-05-20, timeSlot 10:00-12:00
Next Steps for Full Production
Add phone OTP verification UI and backend checks.
Implement Firestore transactions for strict duplicate slot prevention.
Add admin moderation workflows and analytics charts.
Add push notification triggers for approval/rejection.
Add search/filter/history/profile screens.
⚙️ Installation
Clone the Repository
---git clone https://github.com/your-username/grama-anagana.git
Navigate to Project Folder
---cd grama-anagana
Install Dependencies
---npm install
▶️ Run the Project
---npm start
For backend:
---npm run server
