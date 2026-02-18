# Flashcard App - Android Project

![Kotlin](https://img.shields.io/badge/Kotlin-1.17.0-7F52FF?logo=kotlin) ![Jetpack Compose](https://img.shields.io/badge/Jetpack_Compose-2024.10.00-4285F4?logo=jetpackcompose) ![MVI Architecture](https://img.shields.io/badge/Architecture-MVI-FF6F61) ![Room DB](https://img.shields.io/badge/Room-2.8.4-3DDC84?logo=android) ![Dagger Hilt](https://img.shields.io/badge/Dagger_Hilt-2.51.1-007396?logo=dagger) ![Coroutines & Flow](https://img.shields.io/badge/Coroutines_&_Flow-blue?logo=kotlin)

This repository serves as a showcase for a modern, offline-first Android flashcard application. The source code is private, and this document details the architecture and technology stack.

The app is currently in development. I continuously add new features, improving performance and stability.

## About The Project

This application provides a seamless and intuitive experience for creating, organizing, and studying flashcards. It is designed with a focus on a clean user interface, a reactive data flow, and a robust, scalable architecture.

### Key Features

*   **Full Content Management:** Create, read, update, and delete decks, flashcards, and organizational tags.
*   **Offline-First:** The application is fully functional without an internet connection, ensuring data is always available.
*   **Context-Aware UI:** The user interface dynamically adapts to user actions, presenting relevant options for searching, sorting, and bulk-editing content.
*   **Advanced Interactions:** Includes an intuitive multi-select mode for batch operations and the ability to attach images to flashcards.
*   **Consistent UX:** Creation and editing tasks are handled through a consistent and user-friendly bottom sheet interface.

## Architecture & Technology

The application is built on a modern Android architecture that emphasizes separation of concerns, testability, and a unidirectional data flow.

### MVI (Model-View-Intent)

The core architecture follows the MVI pattern, providing a predictable state management loop. User actions are treated as intents, which are processed to produce an immutable state. The UI is a direct function of this state, ensuring consistency and simplifying debugging.

### Tech Stack

*   **UI Toolkit:** **Jetpack Compose** is used for the entire UI, creating a reactive and modern user experience.
*   **Architecture:** **MVI**, **MVVM**, and **Repository Pattern**.
*   **Asynchronicity:** **Kotlin Coroutines & Flow** are used throughout the app for managing background tasks and providing reactive data streams from the local database to the UI.
*   **Dependency Injection:** **Dagger Hilt** manages dependencies, simplifying the architecture and improving testability.
*   **Local Storage:** **Room** provides robust, offline-first data persistence, while **DataStore** handles user preferences.
*   **Navigation:** **Compose Navigation** handles all in-app navigation within a single-activity structure.
*   **Image Loading:** **Coil** efficiently loads and displays images.

### Screenshots

<p align="center">
<img width="281.6" height="594.8" alt="Screenshot_20260217_010946" src="https://github.com/user-attachments/assets/4c23796a-e438-4920-b445-e0b047c84458" />
<img width="281.6" height="594.8" alt="Screenshot_20260217_010729" src="https://github.com/user-attachments/assets/7d734ac4-70c8-41fe-8fc7-80891bb84ca5" />
  <br/>
  <br/>
<img width="281.6" height="594.8" alt="Screenshot_20260215_020521" src="https://github.com/user-attachments/assets/916fb038-ec3e-45fc-9f67-6ea34d5e2761" />
<img width="281.6" height="594.8" alt="Screenshot_20260217_010339" src="https://github.com/user-attachments/assets/bee9cc02-f283-4cc5-a5a6-e105730fad6e" />

## Contact

Balázs Völcsei – [LinkedIn](https://www.linkedin.com/in/balazs-volcsei/) – balazs.volcsei@gmail.com
