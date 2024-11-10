# 📱 Highland Haul User End

**Highland Haul** is a mobile application built using React Native, designed specifically for University of Toronto Scarborough (UTSC) community members. The app aims to offer a sustainable, accessible, and time-efficient ridesharing solution tailored for students and staff who face long and inconvenient commutes.

## 🚀 Features

- **UTORID Authentication**: Secure login using UTORID ensures that only certified UTSC members can use the app.
- **Passenger Flow**: Users can easily request rides to and from campus using their current location and desired destination.
- **Driver Flow**: Verified drivers can select passengers, view routes, and track their earnings from trips.
- **Accessibility Support**: Drivers are trained based on the GO Transit Accessibility Guide to accommodate seniors, individuals with mobility disabilities, and those with service animals.
- **Safety Measures**: All users are verified UTSC members, creating a safer and more trusted ridesharing experience.
- **Real-time Matching**: The app leverages common student schedules to match riders and drivers efficiently.

## 📦 Tech Stack

- **Frontend**: React Native
- **Backend**: Node.js (Express)
- **Authentication**: UTORID-based authentication
- **Database**: Firebase/Firestore (for user data, ride requests, and ride history)
- **Maps & Location Services**: Google Maps API

## ⚙️ Installation

To set up the project locally, follow these steps:

### Prerequisites

- [Node.js](https://nodejs.org/) (v18 or higher)
- [Yarn](https://yarnpkg.com/) or [npm](https://www.npmjs.com/)
- [React Native CLI](https://reactnative.dev/docs/environment-setup)
- Android Studio / Xcode (for Android/iOS development)
- Firebase Project for database and authentication

### Steps

1. **Clone the repository:**

   ```bash
   git clone https://github.com/yourusername/highland-haul.git
   cd highland-haul
   ```

2. **Install dependencies:**

   ```bash
   yarn install
   ```

   Or, if you use npm:

   ```bash
   npm install
   ```

3. **Set up Firebase:**

   - Create a Firebase project at [Firebase Console](https://console.firebase.google.com/).
   - Add Android and iOS apps to your Firebase project.
   - Download the `google-services.json` (Android) and `GoogleService-Info.plist` (iOS) files.
   - Place these files in the respective platform folders:
     - `android/app/google-services.json`
     - `ios/GoogleService-Info.plist`

4. **Configure environment variables:**

   Create a `.env` file in the root directory:

   ```
   GOOGLE_MAPS_API_KEY=your_google_maps_api_key
   FIREBASE_API_KEY=your_firebase_api_key
   FIREBASE_AUTH_DOMAIN=your_firebase_auth_domain
   FIREBASE_PROJECT_ID=your_firebase_project_id
   FIREBASE_STORAGE_BUCKET=your_firebase_storage_bucket
   FIREBASE_MESSAGING_SENDER_ID=your_firebase_messaging_sender_id
   FIREBASE_APP_ID=your_firebase_app_id
   ```

   **Note:** Make sure to keep this file secure and never share it publicly.

5. **Run the app:**

   - For Android:

     ```bash
     npx react-native run-android
     ```

   - For iOS:

     ```bash
     npx react-native run-ios
     ```

## 📖 Usage

### Passenger Flow

1. Login using your UTORID.
2. Fill out your personal information (name, email, preferred ride times).
3. Enable location services and book your ride.
4. Choose your destination (to campus or home).
5. Track your ride in real-time and view estimated arrival time.

### Driver Flow

1. Complete the driver registration (driving experience, license, criminal record check).
2. Login using your UTORID.
3. View available passengers and select a ride request.
4. Start the trip and follow the route on the map.
5. Track your earnings and view ride history.

## 🔍 App Demo

**Video Demo:** [Link to demo video]

## 📚 Documentation

For detailed documentation, including API endpoints and data models, refer to the [docs/](docs/) folder.
