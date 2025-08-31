# Architecture Overview

This project follows a modular full-stack architecture with clear separation of concerns between the frontend, backend, and database.

## High-Level App Structure

### 1. Frontend (Expo + TypeScript)
    - Built with Expo for cross-platform support (iOS & Android).
    - Handles user interactions such as:
        - Browsing and searching for local cooks.
        - Viewing cook profiles, menus, and ratings.
        - Booking meals or services.
        - Managing user accounts and preferences.
    - Uses EAS Build for production deployment.

### 2. Backend (Spring Boot)
    - REST API built with Spring Boot.
    - Core features:
        - User authentication & authorization (JWT-based).
        - Cook and customer management.
        - Location-based search for nearby cooks.
        - Booking & order management.
        - Ratings and reviews system.
    - Integrates with a relational database for persistence.

### 3. Database
    - Relational database (e.g., PostgreSQL or MySQL).
    - Stores structured data:
        - Users (cooks and customers).
        - Menus & meal listings.
        - Orders & bookings.
        - Reviews & ratings.
        - Payment or transaction history (if integrated).

### 4. Authentication Layer
    - Supports both form login and OAuth2 login (Google, Facebook).
    - Issues JWT tokens to authenticate API requests.


### 5. DevOps / Tooling
    - GitHub for version control, CI/CD, and issue tracking.
    - Docker (optional) for consistent local environment setup.
    - Unit & integration testing across backend and frontend.

## System Diagram

```mermaid
flowchart TD
    subgraph Frontend["Frontend - Expo (React Native + TypeScript)"]
        UI[UI Components]
        SM[State Management]
        API[API Calls]
    end

    subgraph Backend["Backend - Spring Boot"]
        AUTH[Auth Layer (JWT/OAuth2)]
        BL[Business Logic]
        REST[REST Controllers]
    end

    subgraph Database["Database - PostgreSQL/MySQL"]
        Tables[(Users, Cooks, Meals, Orders, Locations)]
    end

    UI --> API --> REST
    REST --> BL --> Tables
    AUTH --> REST
```





docs/architecture.md → this is where the High-Level App Structure (Expo frontend, Spring Boot backend, DB, etc.) with diagrams if possible.