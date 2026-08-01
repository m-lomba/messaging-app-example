# Android Real-Time Messaging App Example (Java)

An Android reference application demonstrating a real-time messaging interface powered by **Firebase Authentication** and **Firebase Realtime Database** in Java.

## Overview
This project showcases the implementation of a real-time chat architecture in native Android Java. It combines user authentication with real-time data sync to handle chat sessions, message rendering via `RecyclerView`, and dynamic message data modeling.

## Key Features
* **Real-Time Data Sync:** Instant message transmission and listener updates using `firebase-database:20.0.2`.
* **User Session Management:** Authentication handling via `firebase-auth:21.0.1` to attribute messages to users.
* **Chat UI & List Management:** Custom `RecViewAdapter` implementation for rendering message threads using a `Message` data model.
* **Multi-Activity Flow:** Navigation handling between active user lists/lobby (`MainActivity`) and direct messaging rooms (`ChatActivity`).

## Architecture & Project Structure
```
com.example.messagingappexample/
├── MainActivity.java
├── ChatActivity.java
├── RecViewAdapter.java
└── Message.java
```

## Tech Stack
* **Language:** Java 8
* **Backend Services:** Firebase Realtime Database, Firebase Authentication
* **UI Components:** `androidx.recyclerview`, `ConstraintLayout`, Material Components
* **Min SDK:** 16 (Android 4.1)
* **Target SDK:** 30

## Quick Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/m-lomba/messaging-app-example.git
   ```
2. Open the project in **Android Studio**.
3. Register the app in your [Firebase Console](https://console.firebase.google.com/) and place your `google-services.json` file inside the `app/` directory.
4. Enable **Firebase Authentication** and **Realtime Database** in the console.
5. Build and run on an emulator or physical device running API 16 or higher.
