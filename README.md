# Tunisia Touristic — Intelligent Tourist Guide (Mobile App)

## I. Project Overview
**Tunisia Touristic** is a **Flutter** mobile application designed to help both **tourists** and **locals** discover Tunisia’s popular and hidden destinations.  
The platform offers real-time location services, destination search, favorites, ratings, and publication management by administrators.

---

## II. Existing Solutions
Travelers have always explored Tunisia, but existing solutions are limited:
- Popular destinations are well known, but hidden gems remain hard to find.
- Information is scattered or incomplete.
- Users often fear getting lost or struggle to organize their trip.

---

## III. Problem Statement
- Lack of centralized, reliable information on destinations.
- Difficulty selecting the best destination.
- Need for geolocation and real-time navigation.
- No unified platform for sharing and rating destinations.

**Tunisia Touristic** addresses these challenges by providing a **smart mobile guide** with geolocation, real-time data, and user interaction.

---

## IV. Project Requirements

### Objective
Provide a mobile guide that:
- Centralizes tourist destination information.
- Offers search, filtering, and real-time geolocation.
- Allows users to add, rate, and save destinations.
- Enables administrators to manage and validate content.

### Target Users
- **Users**: Tourists and Tunisians looking to explore.
- **Administrator**: Manages publications and user requests.
- **Visitors**: Can browse destinations without authentication.

---

## V. Functional Description

### Administrator
- Secure authentication (JWT).
- Manage user requests and submissions.
- Create, update, and delete destinations.

### Registered User
- Sign up / Log in / Log out.
- Browse and search destinations.
- View destination details (images, description, map).
- Add a new destination (with moderation).
- Manage profile (avatar, language preferences).
- Add/remove destinations to **favorites**.
- Rate the app and destinations.
- Detect current location and calculate distances.
- Change app language.

### Visitor (Non-authenticated)
- View destinations and details only.

---

## VI. Key Features & Technologies
- **Flutter**: Cross-platform mobile development (Android & iOS).
- **Firebase Firestore**: Real-time NoSQL database to store destinations, users, favorites, ratings, and comments.
- **Firebase Authentication**: Secure user login with email/password or social providers.
- **Firebase Cloud Messaging (FCM)**: Push notifications for new destinations or updates.
- **Google Maps API**: Interactive map with geolocation and route visualization.
- **JWT**: Token-based authentication for admin panel (if backend is separate).
- **Firestore Security Rules**: Role-based access to collections (admin/user/visitor).

---

## VII. Non-Functional Requirements
- **Security**: Role-based Firestore rules and JWT for secure access.
- **Scalability**: Firestore supports large data volumes with real-time updates.
- **Usability**: Clean UI/UX optimized for mobile.
- **Availability**: High uptime with Firebase hosting and services.
- **Performance**: Fast response times with Firestore real-time sync.
- **Extensibility**: Easy integration of APIs (weather, travel news, recommendations).

---

## VIII. Installation & Setup

### Prerequisites
- [Flutter SDK](https://flutter.dev/docs/get-started/install)
- Firebase project (Firestore, Authentication, Cloud Messaging enabled)
- Google Maps API key

### Steps
1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/tunisia-touristic.git
   cd tunisia-touristic
