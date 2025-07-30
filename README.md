# Kasungu Agricultural Weather Mobile App

A React Native mobile application that provides real-time weather data, disease alerts, and farming recommendations specifically for Kasungu District, Malawi.

## Features

### 🌤️ Real-Time Weather Data
- Current weather conditions for Kasungu District
- 7-day detailed weather forecast
- Temperature, humidity, rainfall, and wind speed data
- Weather condition icons and descriptions

### 📊 Interactive Charts
- Temperature trend visualization
- Rainfall forecast charts
- Historical weather patterns

### ⚠️ Smart Alerts
- Disease risk assessments based on weather conditions
- Crop-specific disease alerts for maize, tobacco, groundnuts, sweet potatoes, and soybeans
- Push notifications for critical weather events
- Severity-based alert system (High, Medium, Low)

### 🌾 Farming Recommendations
- Weather-based farming activity suggestions
- Seasonal planting and harvesting guidance
- Crop-specific recommendations
- Priority-based activity planning

### 🔧 Customizable Settings
- English and Chichewa language support
- Notification preferences
- Data caching and offline support
- Location-based weather data

## Installation

### Prerequisites
- Node.js (v16 or higher)
- Expo CLI
- Android Studio (for Android development)
- Xcode (for iOS development, macOS only)

### Setup Instructions

1. **Clone the repository**
   \`\`\`bash
   git clone <repository-url>
   cd kasungu-weather-mobile
   \`\`\`

2. **Install dependencies**
   \`\`\`bash
   npm install
   \`\`\`

3. **Configure API Key**
   - Get a free API key from [OpenWeatherMap](https://openweathermap.org/api)
   - Replace `your_openweather_api_key_here` in `src/services/WeatherService.ts`

4. **Start the development server**
   \`\`\`bash
   npm start
   \`\`\`

5. **Run on device/simulator**
   \`\`\`bash
   # For Android
   npm run android
   
   # For iOS
   npm run ios
   \`\`\`

## Building for Production

### Android APK (for testing)
\`\`\`bash
eas build --platform android --profile preview
\`\`\`

### Android App Bundle (for Play Store)
\`\`\`bash
eas build --platform android --profile production
\`\`\`

### iOS (for App Store)
\`\`\`bash
eas build --platform ios --profile production
\`\`\`

## App Structure

\`\`\`
src/
├── screens/           # Main app screens
│   ├── HomeScreen.tsx
│   ├── ForecastScreen.tsx
│   ├── AlertsScreen.tsx
│   ├── RecommendationsScreen.tsx
│   └── SettingsScreen.tsx
├── services/          # Business logic and API calls
│   ├── WeatherService.ts
│   ├── NotificationService.ts
│   └── StorageService.ts
└── theme/             # App styling and theme
    └── theme.ts
\`\`\`

## Key Technologies

- **React Native**: Cross-platform mobile development
- **Expo**: Development platform and build service
- **React Navigation**: Navigation library
- **React Native Paper**: Material Design components
- **React Native Chart Kit**: Data visualization
- **AsyncStorage**: Local data persistence
- **Expo Notifications**: Push notifications
- **Expo Location**: GPS location services

## Weather Data Integration

The app integrates with OpenWeatherMap API to provide:
- Real-time weather conditions
- 7-day weather forecasts
- Location-based weather data for Kasungu District
- Automatic data caching for offline use

## Notification System

### Daily Notifications
- Morning weather summary (6:00 AM)
- Evening farming tips (6:00 PM)

### Alert Notifications
- Extreme weather warnings
- High-risk disease alerts
- Critical farming activity reminders

## Offline Support

The app includes robust offline functionality:
- Cached weather data
- Stored farming recommendations
- Offline disease alert database
- Local settings persistence

## Localization

The app supports both English and Chichewa languages:
- UI text translation
- Weather condition descriptions
- Farming terminology
- Cultural adaptation for local farming practices

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly on both Android and iOS
5. Submit a pull request

## Support

For technical support or feature requests:
- Email: agriculture@kasungu.gov.mw
- Phone: +265-1-250-123

## License

© 2024 Kasungu District Agricultural Office. All rights reserved.

This application is developed to support farmers in Kasungu District with weather intelligence and agricultural guidance.
\`\`\`

Finally, let's create a deployment script:
