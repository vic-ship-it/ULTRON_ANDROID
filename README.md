# ULTRON Android Assistant

ULTRON is an Android application that acts as a voice-controlled personal assistant for device actions such as app launching, calling, messaging, camera access, settings navigation, and accessibility-based UI interaction.

This repository contains the Android app source and a GitHub Actions workflow for building the debug APK.

## Features

- Voice-driven assistant interaction
- Open installed apps and common system apps
- Make phone calls and open SMS flow
- Open camera and toggle flashlight
- Control volume and ringer modes
- Check battery, time, and date
- Open device settings pages
- UI automation using Android Accessibility Service
- Support for app and system navigation commands

## Project Structure

```text
ULTRON_ANDROID/
├── .github/
│   └── workflows/
│       ├── android-build.yml
│       └── android.yml
├── app/
│   ├── build.gradle
│   └── src/
│       ├── main/
│       │   ├── AndroidManifest.xml
│       │   ├── AndroidManifest.xml.before_contacts
│       │   ├── AndroidManifest.xml.before_new_17
│       │   ├── AndroidManifest.xml.before_remaining_features
│       │   ├── java/
│       │   │   └── com/
│       │   │       └── ultron/
│       │   │           └── assistant/
│       │   │               ├── MainActivity.java
│       │   │               ├── accessibility/
│       │   │               ├── actions/
│       │   │               ├── communication/
│       │   │               ├── core/
│       │   │               └── voice/
│       │   └── res/
│       │       ├── values/
│       │       └── xml/
├── build.gradle
├── settings.gradle
├── test-java.sh
├── .gitignore
├── add_17_methods.py
└── README.md
