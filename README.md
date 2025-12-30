# Sportify

An Android application built with Java for sports enthusiasts.

## About

Sportify is a feature-rich native Android application that combines social networking, real-time interactions, and advanced analytics in the sports domain. Built with Java, this comprehensive platform demonstrates modern Android development practices including real-time data synchronization, machine learning integration, and seamless multimedia handling.

The application showcases a full-stack mobile solution with real-time commenting, interactive rating systems, location-based features, and AI-powered predictions using TensorFlow Lite. With robust user authentication, dynamic content management, and professional reporting capabilities, Sportify serves as both a functional sports platform and a demonstration of enterprise-level Android development techniques.

## Features

### Core Social Features
- 💬 **Real-time Commenting System** - Post and view comments instantly without page refresh
- 👍👎 **Like/Dislike System** - Interactive engagement with real-time counter updates
- ⭐ **Live Rating System** - Dynamic rating functionality for posts and content
- 📄 **Smart Pagination** - Efficient content browsing with paginated views

### User Management & Verification
- ✅ **Real-time Username Validation** - Instant unique username verification without page reload
- 📧 **Email & Phone Verification** - Secure multi-channel user verification system
- 🔐 **Session Management** - Secure login/logout with session handling

### Media & Content
- 🎵 **Embedded Media Player** - Play YouTube videos and external audio/video content
- 📸 **Image/File Upload** - Upload and display user-generated content
- 🗺️ **Google Maps Integration** - Real-time location tracking and embedded maps

### AI & Advanced Features
- 🤖 **TensorFlow Lite Integration** - Real-time ML predictions and analysis
- 📊 **Crystal Reports** - Professional reporting and data visualization
- 🔌 **RESTful & SOAP APIs** - Comprehensive API integration support
- 📈 **GraphQL Implementation** - Efficient data querying and manipulation

### UI/UX Enhancements
- 📅 **Date Picker** - Intuitive date selection interface
- ✨ **GSAP Animations** - Smooth, engaging UI animations
- 🎨 **SASS Styling** - Modern, maintainable CSS architecture
- 📱 **Dynamic Forms** - Multiple text boxes and dropdown list handling

### Development & Architecture
- 🗄️ **Entity Relationship Design** - Well-structured database architecture
- 🔧 **Modern Workflow Tools** - Git, Webpack, and build automation integration
- 🏗️ **Scalable Architecture** - Clean code structure following best practices

## Technologies Used

- **Language:** Java
- **Platform:** Android
- **Build Tool:** Gradle
- **Development IDE:** Android Studio

### Key Libraries & Dependencies

**Core Android Libraries:**
- AndroidX Libraries (Material Design, RecyclerView, CardView)
- Session Management (SharedPreferences)

**Networking & APIs:**
- Retrofit / OkHttp - RESTful API integration
- SOAP Client - SOAP API communication
- GraphQL Client - Efficient data querying

**Database:**
- Room Database / SQLite - Local data persistence
- Real-time Database Integration

**Media & UI:**
- Glide / Picasso - Image loading and caching
- ExoPlayer / MediaPlayer - Audio/video playback
- YouTube Android Player API - Embedded video streaming
- Material Date Picker - Date selection

**Maps & Location:**
- Google Maps SDK - Map integration and location services
- Google Play Services Location API

**Machine Learning:**
- TensorFlow Lite - On-device ML inference
- TensorFlow Lite Support Library

**Reporting:**
- Crystal Reports Integration - Data reporting

**Animation:**
- GSAP (GreenSock Animation Platform) - Advanced animations
- Android Animation API

**Styling:**
- SASS/SCSS - Enhanced CSS preprocessing

**Development Tools:**
- Git - Version control
- Webpack / Gradle - Build automation
- Android Debug Bridge (ADB)

## Prerequisites

Before you begin, ensure you have the following installed:

- **Android Studio** (Latest stable version recommended)
  - Download from: https://developer.android.com/studio
- **Java Development Kit (JDK)** 8 or higher
- **Android SDK** with appropriate API levels
- **Git** for version control

## Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/preaus007/Sportify.git
   ```

2. **Open the project in Android Studio**
   - Launch Android Studio
   - Select "Open an Existing Project"
   - Navigate to the cloned repository folder
   - Click "OK" and wait for Gradle sync to complete

3. **Configure the project**
   - Ensure you have the required SDK versions installed
   - Sync project with Gradle files
   - Update any dependencies if prompted

4. **Run the application**
   - Connect an Android device via USB with Developer Options enabled
   - Or start an Android Virtual Device (AVD) from AVD Manager
   - Click the "Run" button (green play icon) in Android Studio
   - Select your target device

## Project Structure

```
Sportify/
├── app/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/
│   │   │   │   └── [your package structure]
│   │   │   ├── res/
│   │   │   │   ├── layout/
│   │   │   │   ├── drawable/
│   │   │   │   ├── values/
│   │   │   │   └── ...
│   │   │   └── AndroidManifest.xml
│   │   └── androidTest/
│   ├── build.gradle
│   └── proguard-rules.pro
├── gradle/
├── build.gradle
├── settings.gradle
├── gradlew
├── gradlew.bat
└── README.md
```

## Usage

### Getting Started
1. **Registration & Login**
   - Register with email/phone verification
   - Real-time username availability check during registration
   - Secure session-based authentication

2. **Main Features**

   **Social Interactions:**
   - Browse posts with smart pagination
   - Add comments in real-time without page refresh
   - Like/dislike posts and see live counter updates
   - Rate content using the interactive rating system

   **Content Management:**
   - Upload images and files to your profile or posts
   - Embed and play YouTube videos directly in the app
   - Use date picker for scheduling or event creation
   - Fill dynamic forms with multiple inputs and dropdowns

   **Location Features:**
   - View Google Maps with real-time location tracking
   - Explore embedded maps for events or venues

   **AI Features:**
   - Experience real-time predictions powered by TensorFlow Lite
   - Get intelligent recommendations based on ML models

   **Reporting:**
   - Generate and view Crystal Reports for analytics
   - Access comprehensive data visualizations

3. **Tips**
   - All real-time features work without refreshing the page
   - Comments and reactions appear instantly
   - Username validation prevents duplicate accounts
   - Session persists across app restarts until logout

## Configuration

### API Keys Configuration

1. Create a `local.properties` file in the root directory (if not exists)
2. Add your API keys and configuration:
   ```properties
   # Google Maps API Key
   MAPS_API_KEY="your_google_maps_api_key"
   
   # YouTube Data API Key
   YOUTUBE_API_KEY="your_youtube_api_key"
   
   # Backend API Configuration
   API_BASE_URL="your_api_base_url"
   
   # GraphQL Endpoint
   GRAPHQL_ENDPOINT="your_graphql_endpoint"
   
   # SOAP API Endpoint
   SOAP_ENDPOINT="your_soap_endpoint"
   ```

3. Add API key to `AndroidManifest.xml` (for Google Maps):
   ```xml
   <meta-data
       android:name="com.google.android.geo.API_KEY"
       android:value="${MAPS_API_KEY}" />
   ```

### Database Configuration
- Configure your database connection endpoints in the app configuration
- Update database URLs for real-time features (comments, likes, username validation)

### TensorFlow Lite Model
- Place your `.tflite` model files in `app/src/main/assets/`
- Update model file names in the prediction service configuration

### Email/SMS Verification
- Configure email service provider credentials
- Set up SMS gateway API keys for phone verification

**Note:** Never commit `local.properties` or files containing sensitive credentials to version control. Add them to `.gitignore`.

## Testing

Run unit tests:
```bash
./gradlew test
```

Run instrumented tests:
```bash
./gradlew connectedAndroidTest
```

## Acknowledgments

- **Google** - For Maps SDK, Play Services, and TensorFlow Lite
- **YouTube API** - For embedded video streaming capabilities
- **GreenSock (GSAP)** - For powerful animation library
- **Retrofit & OkHttp** - For robust networking solutions
- **Crystal Reports** - For professional reporting tools
- **Open Source Community** - For various libraries and tools that made this project possible

## Contact

**Project Maintainer:** Touhedul Islam

- GitHub: [@preaus007](https://github.com/preaus007)
- Project Link: [https://github.com/preaus007/Sportify](https://github.com/preaus007/Sportify)

---
