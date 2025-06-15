---
title: Smart Intersections
publishDate: 2025-04-07 00:00:00
img: /assets/borInter.png
img_alt: Smart Intersections app interface showing an interactive map and notifications
description: |
  Smart Intersections is an Android mobile application designed to improve road safety in Bordeaux. By leveraging Bordeaux Métropole’s open data, this app provides an interactive visualization of critical intersections, a detailed list of roadworks, and a customizable alert system to notify users in real time.
tags:
  - Android
  - Road Safety
  - Open Data
  - Android Studio
---

### Smart Intersections – Mobile App for Road Safety

##### Description
Smart Intersections is a mobile application developed with Android Studio to enhance road safety in Bordeaux. It uses Bordeaux Métropole’s open data to inform users about critical intersections and ongoing roadworks, and offers personalized alerts.

##### Features
- **Interactive Map**: Geolocated display of intersections and roadworks using the Google Maps SDK for native, high-performance integration.  
- **Roadworks List**: Detailed view of work zones with search, filter, and sort capabilities (by distance and work type).  
- **Alert System**: Contextual notifications based on proximity to roadworks, with customizable settings and alert history.

##### Requirements
- Android Studio & Android SDK (Android 13 / API 33)  
- Emulator or compatible Android device (e.g., Pixel 8)  
- Internet connection and location permissions  

##### Installation

1. **User Installation**:  
   - Download the APK from the official site.  
   - Allow installation from unknown sources.  
   - Install the app on your device.  
   - On first launch, grant the required permissions (location, network access).

2. **Development Setup**:  

   - git clone https://github.com/lamiaeJbira/BordeauxIntersections.git
   - cd BordeauxIntersections


* Open the project in Android Studio.
* Build and run the app on an emulator or connected device.

##### Usage

The app is organized into three main tabs:

* **Map**: Interactive view of intersections and roadworks with auto-zoom and built-in controls.
* **List**: Detailed listing of roadworks with search, filter, and sort options.
* **Alerts**: Configuration of proximity-based notifications and review of past alerts.

##### Testing & Validation

Tested on a Pixel 8 emulator running Android 13, including:

* Location accuracy verification
* Contextual alert triggering validation
* Performance tests for map loading and data handling

