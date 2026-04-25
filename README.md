# Inventory Pro: Android Management System

[![License: Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
[![Platform](https://img.shields.io/badge/Platform-Android-green.svg)](https://developer.android.com/)
[![Language](https://img.shields.io/badge/Language-Java-orange.svg)](https://www.java.com/)

## 📝 Project Summary
**Inventory Pro** was developed to solve the critical issue of manual data entry errors and stock mismanagement in small retail environments. Many small businesses rely on paper logs or memory, leading to "stockouts" or over-stocking. This project provides a **local-first mobile solution** that uses barcode scanning for speed and automated SMS alerts to ensure inventory levels are maintained without constant manual checking.

---

## 🚀 Key Features
* **Full CRUD Management:** Seamlessly Create, Read, Update, and Delete inventory items via a SQLite-backed data layer.
* **Barcode Integration:** Integrated hardware interfacing using the **ZXing (Zebra Crossing)** library for rapid SKU and barcode scanning.
* **Proactive SMS Alerts:** Automated stock monitoring that triggers the Android Telephony API to send low-stock notifications based on customizable thresholds.
* **Modern UI/UX:** Built with **Material Design 3**, featuring a responsive, card-based grid system and dynamic UI updates.

---

## 🛠 Tech Stack
| Category | Technology |
| :--- | :--- |
| **Language** | Java |
| **Database** | SQLite (Relational storage with version-controlled migrations) |
| **Architecture** | Android Jetpack (View Binding, Lifecycle components) |
| **UI Framework** | Material Design 3, ConstraintLayout |
| **Libraries** | ZXing (Barcode Scanning), AndroidX AppCompat |

---

## 🧠 Professional Reflection

### What was done particularly well?
The most successful aspect was the **logic integration** between the SQLite data layer and the Android Telephony API. Creating a system that doesn't just store data but *acts* on it—by checking thresholds and automatically triggering a communication service—demonstrated a strong grasp of event-driven mobile development. Additionally, successfully managing a **Version 3 database migration** without data loss shows professional-grade care for data integrity.

### Maintainability, Readability, & Adaptability
I prioritized a clean codebase through several key architectural decisions:
* **Separation of Concerns:** Isolated logic into dedicated helper classes (`DatabaseHelper` and `NotificationHelper`) to make the code easier to debug and update.
* **View Binding:** Utilized View Binding to eliminate boilerplate code, making the Activity and Fragment logic significantly more readable.
* **Resource Management:** Externalized all strings, colors, and dimensions into XML files, making the app adaptable for localization or "Dark Mode" without touching core logic.

### Future Improvements & Roadmap
* **Cloud Synchronization:** Currently, data is siloed on a single device. Moving to a cloud-synced backend (like Firebase) would allow multiple employees to manage inventory in real-time.
* **Unit Testing:** Increasing JUnit test coverage for the helper classes would ensure that future updates don't break the core alert logic.
* **Predictive Analytics:** Expanding the dashboard to include trends based on historical stock movements.

### Transferable Skills
* **Hardware Interfacing:** Connecting software to physical sensors (camera/scanner) is directly applicable to IoT and mobile computer vision.
* **Permission & Security Workflows:** Managing sensitive permissions (SMS and Camera) is a fundamental requirement for secure mobile development.
* **State-Driven UI:** Designing interfaces that update dynamically based on real-time database states—a blueprint for modern full-stack development.

---

## ⚙️ Getting Started
1.  **Clone the Repository:**

2.  **Open in Android Studio:**
    Ensure you have the latest version of Android Studio and the Android SDK installed.
3.  **Sync Gradle:**
    Allow the project to resolve dependencies for ZXing and AndroidX.
4.  **Run:**
    Deploy to a physical device or emulator. *(Note: SMS features require a device with an active SIM/telephony support).*

---

## 📄 License
This project is part of my professional portfolio and is intended for educational purposes. Licensed under the **Apache 2.0 License**.
