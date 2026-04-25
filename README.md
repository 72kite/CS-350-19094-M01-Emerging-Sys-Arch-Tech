# Inventory Pro: Android Management System
    
    [![License: Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
    [![Platform](https://img.shields.io/badge/Platform-Android-green.svg)](https://developer.android.com/)
    [![Language](https://img.shields.io/badge/Language-Java-orange.svg)](https://www.java.com/)
    
    **Inventory Pro** is a robust Material 3 mobile application designed to eliminate manual stock-tracking errors for small businesses and individual retailers. By utilizing a local-first architecture, it ensures high performance and data privacy while providing proactive alerts to prevent stockouts.
    
    ## 🚀 Key Features
    * **Full CRUD Management:** Seamlessly Create, Read, Update, and Delete inventory items via a SQLite-backed data layer.
    * **Barcode Integration:** Integrated hardware interfacing using the **ZXing (Zebra Crossing)** library for rapid SKU and barcode scanning.
    * **Proactive SMS Alerts:** Automated stock monitoring that triggers the Android Telephony API to send low-stock notifications based on customizable thresholds.
    * **Modern UI/UX:** Built with **Material Design 3**, featuring a responsive, card-based grid system and dynamic UI updates.
    
    ---
    
    ## 🛠 Tech Stack
    * **Language:** Java
    * **Database:** SQLite (Relational storage with version-controlled schema migrations)
    * **Architecture:** Android Jetpack (View Binding, Lifecycle components)
    * **UI Framework:** Material Design 3, ConstraintLayout
    * **Libraries:** ZXing (Barcode Scanning), AndroidX AppCompat
    
    ---
    
    ## 🧠 Project Reflection
    
    ### Successes & Technical Wins
    I am particularly proud of the integration between the data layer and the user interface. Specifically, implementing the logic that bridges the SQLite database states with the Android Telephony API to trigger SMS alerts. I also handled a significant technical hurdle effectively by managing database schema migrations (bumping to Version 3) to ensure that new metadata like "item descriptions" and "minimum stock levels" were supported without crashing the existing user experience.
    
    ### Challenges & Future Roadmap
    * **Cloud Synchronization:** Currently, data is siloed on a single device; enabling multi-user synchronization (e.g., via Firebase or a REST API) would make this app viable for larger warehouse teams.
    * **Predictive Analytics:** I aim to expand the analytics dashboard to include predictive trends based on historical stock movements.
    
    ### Professional Growth & Transferable Skills
    Through this project, I deepened my proficiency with several industry-standard practices:
    * **Permission Handling:** Implementing secure workflows for SMS and Camera permissions, a fundamental requirement for modern mobile development.
    * **Maintainable Architecture:** Adopting **View Binding** to reduce boilerplate and isolating logic into helper classes (`DatabaseHelper`, `NotificationHelper`) to ensure a clean **Separation of Concerns**.
    * **Resource Management:** Externalizing all strings and colors into XML files to support localization and "Dark Mode."
    * **Data-Driven UI:** Designing interfaces that update dynamically based on database states—a blueprint for future full-stack work.
    
    ---
    
    ## 📄 License
    This project is part of my professional portfolio and is intended for educational purposes. Licensed under the Apache 2.0 License.
