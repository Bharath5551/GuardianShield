# 🛡️ GuardianShield – Pre-Incident Safety System

GuardianShield is a mobile safety application designed to detect **pre-incident risk signals** using smartphone sensors and provide **early escalation** before an actual emergency occurs.

**Try it:** [download the Android APK](https://github.com/Bharath5551/GuardianShield/raw/main/app-debug.apk) (debug build; allow installs from unknown sources)

The app focuses on **prevention**, **user control**, and **real-world feasibility**, while strictly following Android security policies.

---

## 🚀 Problem Statement

Most safety applications react **after** an incident occurs.

GuardianShield solves this by:

> Detecting subtle **pre-incident signals** (sudden movements and abnormal behavior patterns) and escalating risk **before** the situation becomes critical.

---

## 🎯 Key Features

### 🔍 Pre-Incident Risk Detection
- Uses the **accelerometer sensor**
- Detects sudden or abnormal movements
- Dynamically increases a **risk score**

### ⚠️ Risk Escalation System
- Continuous monitoring of risk score
- At **80% risk**, Guardian Mode is triggered

### ⏱️ False Alarm Prevention
- 15-second countdown before alert
- User can **cancel alert** to avoid false alarms
- Cancel fully resets the app state

### 🔊 Emergency Feedback
- Loud **emergency siren**
- Strong **vibration pattern**
- Ensures user awareness during escalation

### 📩 Guardian Alert with Live Location
- Emergency SMS with **Google Maps live location**
- Uses system SMS app (Android-compliant & reliable)

### 🧭 First-Time Setup Flow
- One-time setup on first launch
- Guardian phone number (10 digits only)
- Required permissions requested upfront
- Seamless transition to main app

### 📱 Modern UI (Jetpack Compose)
- Material 3 design
- Gradient home screen
- Slide-out dashboard for app status

---

## 🧠 Why SMS Requires User Tap

Android restricts apps from sending SMS silently for security reasons.

GuardianShield complies with Android policy by:
- Opening the system SMS app with message & location pre-filled
- User taps **Send** once to ensure guaranteed delivery

This is the **same approach used by real-world emergency applications**.

---

## 🛠️ Tech Stack

- **Language:** Kotlin  
- **UI:** Jetpack Compose (Material 3)  
- **Sensors:** Accelerometer  
- **Location:** Android LocationManager  
- **Architecture:** Single-Activity Compose  
- **Storage:** SharedPreferences  
- **Minimum SDK:** Android 8.0 (API 26)

---

## 📲 Permissions Used
