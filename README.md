# Cook4Me

## Overview

Cook4Me is a mobile application that connects users with local cooks and chefs who specialize in Nigerian delicacies. Users can discover dishes, explore nearby cooks based on their location, and view cook profiles with ratings, contact options, and social links. Cooks can showcase their meals, manage availability, and attract customers directly through the app.

## Features

- Browse popular Nigerian dishes
- Search for dishes and nearby cooks
- View cook profiles, ratings, and contact options
- Cook dashboard: manage menu, availability, and view reviews

## Tech Stack

- Frontend: React Native with (Expo + EAS)
- Backend: Spring Boot (Java)
- Database: PostgreSQL
- Authentication: JWT / OAuth2 (optional)
- Maps & Geolocation: Google Maps / Mapbox

## Getting Started

### Prerequisites
- Node.js >= 18
- PostgreSQL >= 14
- Yarn or npm
- Expo CLI (npm install -g expo-cli)
- Java 17+ (for Spring Boot)
- Maven or Gradle (Spring Boot build tool)

### Installation

#### Clone the repo
```bash
git clone https://github.com/juliettegodyere/Cook4Me.git
```

#### Install dependencies
cd Cook4Me
yarn install # or npm install

#### Install Frontend (Expo with EAS) dependencies
```bash
cd frontend
# Install dependencies
yarn install   # or npm install

# Run locally with Expo
npx expo start

# For EAS builds (iOS/Android)
# Make sure you have EAS CLI installed globally
npm install -g eas-cli

# Configure project
eas build:configure

# Run build for Android
eas build -p android

# Run build for iOS
eas build -p ios
```

#### Install Backend (Spring Boot) dependencies
```bash
cd backend
# If using Maven
./mvnw clean install
./mvnw spring-boot:run

# If using Gradle
./gradlew build
./gradlew bootRun
```

## Contributing

- [Contribution Guidelines](CONTRIBUTING.md)

## Documentation

- [Architecture Overview](docs/architecture.md)
- [API Documentation](docs/api.md)
- [Database Schema](docs/database-schema.md)
- [Setup Guide](docs/setup-guide.md)

## License

- [MIT License](LICENSE)
