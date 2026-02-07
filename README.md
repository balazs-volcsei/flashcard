# Flashcard App - Android Portfolio Project

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

<img width="140.8" height="297.4" alt="Screenshot_20260207_213429" src="https://github.com/user-attachments/assets/ad13df3d-9740-4c4e-8c5d-cca96d36dc72" />
<img width="140.8" height="297.4" alt="Screenshot_20260207_213329" src="https://github.com/user-attachments/assets/7c10758e-7a28-4317-9dc9-2adc3c74760e" />
<img width="140.8" height="297.4" alt="Screenshot_20260207_213336" src="https://github.com/user-attachments/assets/070dced8-afe0-4cfc-8aee-784d45959c16" />
<img width="140.8" height="297.4" alt="Screenshot_20260207_213445" src="https://github.com/user-attachments/assets/b33fe612-54c4-47a9-ba11-251548f9ff0d" />
<img width="140.8" height="297.4" alt="Screenshot_20260207_213312" src="https://github.com/user-attachments/assets/b10e637f-e87d-4a78-be21-475408df0d82" />


## Contact

Balázs Völcsei – [LinkedIn](https://www.linkedin.com/in/balazs-volcsei/) – balazs.volcsei@gmail.com
