# flutter_sample

A new Flutter project.

## Prerequisites

Before you begin, ensure you have the following installed:

- [Git](https://git-scm.com/downloads)
- [FVM (Flutter Version Management)](https://fvm.app/docs/getting_started/installation)
- Xcode (for iOS development on macOS)
- Android Studio or Android SDK (for Android development)

## Getting Started

### 1. Clone the Repository

```bash
git clone <repository-url>
cd flutter_sample
```

### 2. Install Flutter Version with FVM

This project uses FVM to manage the Flutter SDK version. Install the Flutter version specified in the project:

```bash
fvm install
```

This will install the Flutter version defined in `.fvm/fvm_config.json`.

### 3. Use FVM Flutter

Configure your project to use the FVM-managed Flutter version:

```bash
fvm use
```

### 4. Get Dependencies

Fetch all the project dependencies:

```bash
fvm flutter pub get
```

### 5. Run the App

To run the app on a connected device or simulator:

```bash
# Run on default device
fvm flutter run

# Or list available devices first
fvm flutter devices

# Then run on specific device
fvm flutter run -d <device-id>
```

## IDE Setup

### VS Code

If you're using VS Code, FVM will automatically be detected. You may need to:

1. Install the Flutter and Dart extensions
2. Select the Flutter SDK from `.fvm/flutter_sdk` when prompted
3. Restart VS Code

### Android Studio / IntelliJ

1. Go to `Settings/Preferences` > `Languages & Frameworks` > `Flutter`
2. Set the Flutter SDK path to `<project-root>/.fvm/flutter_sdk`
3. Restart the IDE

## Useful Commands

```bash
# Run with hot reload
fvm flutter run

# Run tests
fvm flutter test

# Build for production
fvm flutter build apk        # Android
fvm flutter build ios        # iOS
fvm flutter build web        # Web

# Analyze code
fvm flutter analyze

# Format code
fvm flutter format .
```

## Resources

- [Flutter Documentation](https://docs.flutter.dev/)
- [FVM Documentation](https://fvm.app/docs)
- [Dart Documentation](https://dart.dev/guides)
