# Flightscry - Flight Itinerary Android App

A proof of concept Android application for Skyscanner's Flightscry project, showcasing a beautiful flight itinerary UI using the Backpack design system.

## Overview

Flightscry is a mobile application that allows users to view their flight itineraries conveniently on their phones. This is a proof of concept (PoC) demonstrating the user interface using dummy flight data.

## Features

- **Flight Information Card**: Displays the flight number
- **Departure Card**: Shows the departure airport code and time
- **Arrival Card**: Shows the arrival airport code and time
- **Backpack UI Components**: Uses Skyscanner's custom Backpack library for consistent, beautiful UI

## Technology Stack

- **Language**: Kotlin
- **Framework**: Android (API 33+)
- **UI Library**: Backpack (Skyscanner's custom UI library)
- **Build System**: Gradle
- **IDE**: Android Studio

## Installation & Setup

### Prerequisites

- Android Studio (Electric Eel or later recommended)
- JDK 11 or later
- Android SDK API 33 (Android Tiramisu)

### Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/Sagark2103/SkyScanner-BackPack-App.git
   cd SkyScanner-BackPack-App
   ```

2. **Open in Android Studio**
   - Open Android Studio
   - File → Open → Select the project directory

3. **Sync Gradle**
   - Android Studio will prompt you to sync Gradle
   - Click "Sync Now" or use the Gradle sidebar

4. **Run the application**
   - Click the green Run button (▶) in the toolbar
   - Select a device (emulator or physical device)
   - The app will build and launch

## Project Structure

```
SkyScanner-BackPack-App/
├── app/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/com/example/flightscry/
│   │   │   │   └── MainActivity.kt
│   │   │   ├── res/
│   │   │   │   ├── layout/
│   │   │   │   │   └── activity_main.xml
│   │   │   │   └── values/
│   │   │   │       └── strings.xml
│   │   │   └── AndroidManifest.xml
│   │   └── test/
│   ├── build.gradle
│   └── proguard-rules.pro
├── build.gradle
├── settings.gradle
└── README.md
```

## Key Files

- **MainActivity.kt**: Main activity that sets the content view to activity_main.xml
- **activity_main.xml**: XML layout file containing the flight information cards using Backpack components
- **build.gradle**: Gradle configuration with Backpack dependency (v43.0.0)

## Components Used

### BpkCardView
A card component from Backpack with customizable corner styles. Used for:
- Flight Information Card
- Departure Card
- Arrival Card

### BpkText
Typography component from Backpack with predefined styles:
- `bpkTextHeading1`: For section titles
- `bpkTextBodyDefault`: For descriptive text

## Sample Data

The app displays dummy flight data for demonstration:
- **Flight Number**: SK452
- **Departure**: LHR (London Heathrow) at 10:30 AM
- **Arrival**: CDG (Paris Charles de Gaulle) at 1:15 PM

## Future Enhancements

- Integration with actual flight data
- Real-time flight status updates
- User authentication
- Booking and reservation features
- Push notifications for flight updates
- Multiple language support

## References

- [Backpack Documentation](https://backpack.github.io/)
- [Android Studio Documentation](https://developer.android.com/studio)
- [Kotlin Documentation](https://kotlinlang.org/docs/home.html)

## License

This project is part of the Skyscanner platform and follows their licensing guidelines.

## Author

Sagar Kulkarni (Sagark2103)

---

**Status**: Proof of Concept (PoC) - UI Showcase Only
