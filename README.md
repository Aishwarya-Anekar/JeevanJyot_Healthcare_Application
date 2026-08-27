# 🏥 JeevanJyot – Healthcare Application

<p align="center">
  <b>A Smart Android-Based Healthcare Application for Patients and Doctors</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Android-green?style=for-the-badge&logo=android" />
  <img src="https://img.shields.io/badge/Language-Java-orange?style=for-the-badge&logo=java" />
  <img src="https://img.shields.io/badge/Android%20SDK-34-blue?style=for-the-badge&logo=android" />
  <img src="https://img.shields.io/badge/Build-Gradle-02303A?style=for-the-badge&logo=gradle" />
</p>

---

## 📌 About the Project

**JeevanJyot** is an Android-based healthcare application designed to provide patients and doctors with a convenient platform for accessing essential healthcare services.

The application brings multiple healthcare utilities together in one place, including **patient and doctor authentication, appointment management, AI-powered health assistance, emergency support, medicine reminders, nearby hospital/pharmacy discovery, location services, and healthcare-related tools**.

The application is developed using **Java and Android SDK** with integrations such as **Google Maps, Google Gemini, Google ML Kit, Volley, OkHttp, and Gson**.

---

## 🎯 Objectives

The main objectives of JeevanJyot are to:

* 🏥 Provide easy access to healthcare-related services
* 👨‍⚕️ Connect patients with doctors
* 📅 Simplify appointment management
* 🤖 Provide AI-based assistance for health-related queries
* 🚨 Provide quick access to emergency assistance
* 💊 Help patients remember their medicines
* 📍 Help users locate nearby hospitals and pharmacies
* 📄 Support healthcare document/report handling
* 📱 Provide a centralized and user-friendly healthcare platform

---

# ✨ Features

## 👤 Patient Module

The patient side of the application provides several healthcare utilities.

### 🔐 Patient Authentication

* Patient login
* Patient registration
* Forgot-password functionality
* Patient profile management

### 🏠 Patient Dashboard

A centralized dashboard gives patients access to the major healthcare services available in the application.

### 🤖 AI Health Chatbot

JeevanJyot includes an AI-powered chatbot integrated with **Google Gemini**.

Users can ask health-related questions such as:

* Symptoms
* Fever
* Cough and cold
* Headache
* Pain
* First aid
* General health queries
* Medicines
* Hospitals and doctors

The application also restricts chatbot interaction to health-related queries and provides a reminder that AI responses should not replace professional medical advice.

> ⚠️ The chatbot is intended for informational assistance and should not be considered a substitute for diagnosis or professional medical consultation.

---

## 🚨 Emergency Assistance

The application provides an emergency assistance feature that can:

* 📞 Initiate an emergency call
* 📩 Send an emergency SMS
* 📍 Retrieve the user's current location
* 🔗 Include a Google Maps location link in the emergency message

The emergency module uses Android's **Call, SMS, and Location permissions** along with Google's Fused Location Provider.

---

## 💊 Medicine Reminder

The medicine reminder feature helps patients remember their medication schedule.

Users can:

* Enter medicine name
* Select reminder time
* Set the duration
* Schedule recurring reminders
* Receive notifications for medicines

The application uses Android's **AlarmManager**, **NotificationChannel**, and **BroadcastReceiver** functionality to implement reminders.

---

## 📍 Find Nearby Hospitals & Pharmacies

JeevanJyot integrates **Google Maps and location services** to help users find nearby healthcare facilities.

Users can:

* 📍 View their current location
* 🔎 Search for a location
* 🏥 Find nearby hospitals
* 💊 Find nearby pharmacies/medical stores
* 🗺️ View locations on Google Maps

The application uses Google Maps, Fused Location Provider, Geocoder, and Places-related functionality.

---

## 👨‍⚕️ Doctor Module

The application also provides functionality for doctors.

Features include:

* Doctor registration
* Doctor login
* Doctor dashboard
* Patient list
* Patient information
* Profile management
* Appointment-related interactions

---

## 📅 Appointment Management

The appointment module provides functionality for interacting with doctors.

It includes options for:

* Booking/scheduling appointments
* Doctor communication
* Calling
* Messaging
* Video meeting access
* Email communication
* Selecting healthcare-related files/documents

---

## 📄 Reports & Prescriptions

The application contains dedicated components for handling:

* Patient reports
* Prescriptions
* Healthcare documents
* File selection and sharing

---

## 💊 Medicine Scanner

The project includes a medicine-scanning component using **Google ML Kit** capabilities.

The project dependencies include ML Kit's:

* Text Recognition
* Barcode Scanning

This can be used as a foundation for extracting or identifying information from medicine-related packaging.

---

# 🛠️ Tech Stack

| Technology                  | Purpose                             |
| --------------------------- | ----------------------------------- |
| **Java**                    | Application development             |
| **Android SDK 34**          | Android development                 |
| **Gradle**                  | Build and dependency management     |
| **AndroidX**                | Android application components      |
| **Material Components**     | UI components                       |
| **ConstraintLayout**        | Responsive UI layouts               |
| **Google Maps SDK**         | Maps and location visualization     |
| **Fused Location Provider** | Current location services           |
| **Google Gemini API**       | AI healthcare chatbot               |
| **Google ML Kit**           | Text recognition & barcode scanning |
| **Volley**                  | Network requests                    |
| **OkHttp**                  | HTTP/API communication              |
| **Gson**                    | JSON parsing                        |
| **Lottie**                  | Animations                          |
| **AlarmManager**            | Medicine reminders                  |
| **Notifications**           | Reminder notifications              |

The current Gradle configuration includes Android SDK 34, minimum SDK 24, View Binding, Google Maps, Location Services, Gemini, ML Kit, Volley, OkHttp, Gson, Material Components, and Lottie.

---

# 🏗️ Project Architecture

The project follows a traditional Android application structure with Java Activities, layouts, adapters, services/utilities, and Android resources.

```text
JeevanJyot_Healthcare_Application/
│
├── app/
│   ├── src/
│   │   └── main/
│   │       ├── java/
│   │       │   ├── LoginActivity.java
│   │       │   ├── DoctorHome.java
│   │       │   ├── PatientHome.java
│   │       │   ├── Appointment.java
│   │       │   ├── Emergency.java
│   │       │   ├── ChatBot.java
│   │       │   ├── GoogleMapsActivity.java
│   │       │   ├── Medicine_Remainder.java
│   │       │   ├── Medicine_Scanner.java
│   │       │   ├── PrescriptionActivity.java
│   │       │   ├── Report.java
│   │       │   ├── PatientListActivity.java
│   │       │   ├── DoctorAdapter.java
│   │       │   ├── AlarmReceiver.java
│   │       │   └── ...
│   │       │
│   │       ├── res/
│   │       │   ├── layout/
│   │       │   ├── drawable/
│   │       │   ├── mipmap/
│   │       │   ├── values/
│   │       │   └── xml/
│   │       │
│   │       └── AndroidManifest.xml
│   │
│   └── build.gradle
│
├── gradle/
├── build.gradle
├── gradle.properties
├── settings.gradle
├── gradlew
└── gradlew.bat
```

The repository contains dedicated Java components for authentication, doctor/patient dashboards, appointments, chatbot functionality, emergency services, maps, medicine reminders, reports, prescriptions, and related utilities.

---

# 🔑 Important Integrations

## 🤖 Google Gemini

The chatbot uses Google's Generative AI SDK to generate responses to health-related user queries.

The application initializes the Gemini model using an API key provided through the application's build configuration.

### Important

Do **not** commit API keys directly to a public GitHub repository.

Use `local.properties`, environment variables, or another secure secrets-management approach.

---

## 🗺️ Google Maps

Google Maps is used for:

* Current location
* Location search
* Map visualization
* Nearby hospital discovery
* Nearby pharmacy discovery

The application requests location permissions and uses Fused Location Provider for location updates.

---

# 📋 Android Permissions

The application uses Android permissions for functionality such as:

* Internet access
* Fine/coarse location
* Notifications
* SMS
* Emergency calling
* Storage/file access
* Network state
* Exact alarms

These permissions are declared in the application's `AndroidManifest.xml`.

> **Security Note:** Review all permissions before deploying the application publicly and request only permissions required for the corresponding feature.

---

# 🚀 Getting Started

## Prerequisites

Before running the project, install:

* **Android Studio**
* **JDK 8 or compatible Android Studio Java environment**
* Android SDK
* Android Emulator or a physical Android device
* Google Maps API key
* Google Gemini API key

The project is configured with **compile SDK 34**, **target SDK 34**, and **minimum SDK 24**.

---

## 1️⃣ Clone the Repository

```bash
git clone https://github.com/Aishwarya-Anekar/JeevanJyot_Healthcare_Application.git
```

```bash
cd JeevanJyot_Healthcare_Application
```

---

## 2️⃣ Open in Android Studio

1. Open **Android Studio**
2. Select **Open**
3. Choose the cloned `JeevanJyot_Healthcare_Application` directory
4. Allow Gradle to sync
5. Install the required Android SDK if prompted

---

## 3️⃣ Configure API Keys

The application uses external APIs including Google Maps and Gemini.

Configure your API credentials securely before running the application.

For example, use a local configuration rather than committing secrets to Git:

```properties
API_KEY=YOUR_GEMINI_API_KEY
```

> Never upload real API keys, passwords, tokens, or private credentials to GitHub.

---

## 4️⃣ Build the Application

From Android Studio:

```text
Build → Make Project
```

Or using Gradle:

### Windows

```bash
gradlew.bat assembleDebug
```

### Linux/macOS

```bash
./gradlew assembleDebug
```

---

## 5️⃣ Run the Application

1. Connect an Android device or start an emulator.
2. Enable USB debugging if using a physical device.
3. Click **Run ▶** in Android Studio.
4. Select your device.
5. Install and launch JeevanJyot.

---

# 🔄 Application Flow

```text
                 ┌───────────────────┐
                 │   JeevanJyot App  │
                 └─────────┬─────────┘
                           │
                    ┌──────▼──────┐
                    │    Login    │
                    └──────┬──────┘
                           │
              ┌────────────┴────────────┐
              │                         │
       ┌──────▼──────┐           ┌──────▼──────┐
       │   Patient   │           │   Doctor    │
       │    Module   │           │   Module    │
       └──────┬──────┘           └──────┬──────┘
              │                         │
     ┌────────┼─────────┐        ┌──────┼───────┐
     │        │         │        │      │       │
     ▼        ▼         ▼        ▼      ▼       ▼
   Chatbot  Emergency  Maps    Patients Appointments
     │        │         │
     ▼        ▼         ▼
   Gemini   SOS/SMS   Hospitals
                     Pharmacies
              │
              ▼
       Medicine Reminder
              │
              ▼
          Notifications
```

---

# 🔐 Security Considerations

Since this application handles healthcare-related functionality, security is especially important.

Recommended improvements before production deployment:

* 🔒 Never hard-code API keys
* 🔒 Use secure authentication
* 🔒 Encrypt sensitive patient information
* 🔒 Avoid storing unnecessary personal information
* 🔒 Use HTTPS for network communication
* 🔒 Validate all user input
* 🔒 Apply least-privilege permissions
* 🔒 Secure emergency contact information
* 🔒 Protect medical reports and prescriptions
* 🔒 Implement proper backend authorization

---

# ⚠️ Medical Disclaimer

JeevanJyot is a **technology project intended to provide healthcare-related assistance and utilities**.

The AI chatbot provides informational responses and should **not be used as a replacement for a qualified medical professional**.

Users should consult a licensed healthcare professional for diagnosis, treatment, medication decisions, or medical emergencies.

In an actual emergency, users should contact the appropriate local emergency services.

---

# 🔮 Future Enhancements

Potential improvements for future versions include:

* [ ] Secure backend integration
* [ ] Real-time doctor-patient chat
* [ ] Video consultation
* [ ] Online appointment scheduling
* [ ] Digital prescription management
* [ ] Secure cloud storage for medical reports
* [ ] Push notifications
* [ ] Improved medicine recognition
* [ ] Multilingual AI healthcare assistance
* [ ] Health-record management
* [ ] Doctor availability tracking
* [ ] Appointment history
* [ ] Improved authentication and authorization
* [ ] Database integration
* [ ] Production-ready API architecture
* [ ] Automated testing
* [ ] CI/CD pipeline

---

# 🧪 Testing

The project includes Android testing dependencies for:

* JUnit
* AndroidX Test
* Espresso

Testing can be expanded to cover:

* Login and registration
* Appointment workflows
* Emergency functionality
* Medicine reminders
* Location services
* Chatbot responses
* Medicine scanning
* Doctor-patient interactions

---

Implementation:


https://github.com/user-attachments/assets/b67087b9-b90c-4f5e-b7c8-6d230e2eb14d


https://github.com/user-attachments/assets/f0892306-8246-4cd9-94f9-1f91f7493af2


https://github.com/user-attachments/assets/d4fc6c2b-9faa-40b2-95ae-fe0f5b1b6e02


https://github.com/user-attachments/assets/7decbfce-8f3e-4fdc-8bc4-22209f8cf1e8


https://github.com/user-attachments/assets/1abf0235-3dd5-474e-ad58-ad0172a050db


https://github.com/user-attachments/assets/6d625ffb-051a-42ee-92f4-8b5639c6cf11



https://github.com/user-attachments/assets/185c2559-f767-4f7b-8bf7-a5a17f6025f7



https://github.com/user-attachments/assets/ec3a3b3f-7486-4edf-9b7d-5c286d8b05ad


https://github.com/user-attachments/assets/66a783c3-125a-4486-9dd4-98302844d37c


