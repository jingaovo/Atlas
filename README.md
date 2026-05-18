# Atlas 🌍

Atlas is a modern, cross-platform travel planning and exploration application built with **Compose Multiplatform**. It allows users to create, manage, and discover trips, pins, and travel experiences with a seamless UI across Android and Desktop.

![App Screenshot](app_screenshot.png)

## Features 🚀

- **Trip Management**: Create and organize trips with detailed itineraries.
- **Interactive Pins**: Mark locations, add photos, and write notes for specific places.
- **Explore Community**: Discover trips shared by other travelers.
- **User Profiles**: Manage your travel preferences, stats, and style.
- **Cross-Platform**: Unified codebase for Android and JVM (Desktop) platforms.
- **Cloud Powered**: Seamless data synchronization using **Supabase** (Auth, Database, and Storage).

## Tech Stack 🛠️

- **Language**: [Kotlin](https://kotlinlang.org/)
- **UI Framework**: [Compose Multiplatform](https://www.jetbrains.com/lp/compose-multiplatform/)
- **Backend**: [Supabase](https://supabase.com/) (PostgreSQL, Auth, Storage)
- **Networking/Serialization**: Kotlinx Serialization, Supabase-kt
- **Architecture**: MVVM (Model-View-ViewModel) with Repository Pattern
- **Dependency Management**: Gradle Version Catalogs

## Project Structure 📁

- `composeApp/src/commonMain`: Shared UI and business logic.
- `composeApp/src/androidMain`: Android-specific implementations and resources.
- `composeApp/src/jvmMain`: Desktop-specific implementations.
- `composeApp/src/commonTest`: Shared unit and integration tests.

## Getting Started 🏁

### Prerequisites
- Android Studio or IntelliJ IDEA
- JDK 17 or higher
- Android SDK (for Android builds)

### Build & Run

#### Android
```bash
./gradlew :composeApp:installDebug
```

#### Desktop (JVM)
```bash
./gradlew :composeApp:run
```

## Backend Configuration ☁️

The project uses Supabase for backend services. Configuration is managed in `SupabaseClient.kt`. For a production setup, ensure your Supabase URL and Key are correctly configured in `local.properties` or environment variables as defined in `build.gradle.kts`.

