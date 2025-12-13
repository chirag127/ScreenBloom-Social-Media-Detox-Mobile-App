<!--
PROTOCOL: This PROPOSED_README.md is a proposal for the new README.md.
It strictly adheres to the directives outlined in AGENTS.md.
All content is generated based on a comprehensive analysis of the repository's
purpose, architecture, and the Apex Technical Authority's 2025/2026 standards.
-->

# ScreenBloom - AI-Powered Social Media Detox & Digital Wellness Mobile App

<p align="center">
  <a href="https://github.com/chirag127/ScreenBloom-Social-Media-Detox-Mobile-App">
    <img src="https://github.com/chirag127.png" alt="ScreenBloom Logo" width="120"/>
  </a>
</p>

<p align="center">
  <a href="https://github.com/chirag127/ScreenBloom-Social-Media-Detox-Mobile-App/actions/workflows/ci.yml">
    <img src="https://img.shields.io/github/actions/workflow/status/chirag127/ScreenBloom-Social-Media-Detox-Mobile-App/ci.yml?branch=main&style=flat-square&logo=github" alt="Build Status"/>
  </a>
  <a href="https://codecov.io/gh/chirag127/ScreenBloom-Social-Media-Detox-Mobile-App">
    <img src="https://img.shields.io/codecov/c/github/chirag127/ScreenBloom-Social-Media-Detox-Mobile-App?style=flat-square&logo=codecov" alt="Code Coverage"/>
  </a>
  <img src="https://img.shields.io/badge/TS-%5E5.3.0-blue?style=flat-square&logo=typescript" alt="Tech Stack: TypeScript"/>
  <img src="https://img.shields.io/badge/ReactNative-%5E0.73.0-61DAFB?style=flat-square&logo=react" alt="Tech Stack: React Native"/>
  <img src="https://img.shields.io/badge/Expo-%5E50.0-000000?style=flat-square&logo=expo" alt="Tech Stack: Expo"/>
  <a href="https://github.com/chirag127/ScreenBloom-Social-Media-Detox-Mobile-App/blob/main/LICENSE">
    <img src="https://img.shields.io/github/license/chirag127/ScreenBloom-Social-Media-Detox-Mobile-App?style=flat-square" alt="License: CC BY-NC 4.0"/>
  </a>
  <a href="https://github.com/chirag127/ScreenBloom-Social-Media-Detox-Mobile-App/stargazers">
    <img src="https://img.shields.io/github/stars/chirag127/ScreenBloom-Social-Media-Detox-Mobile-App?style=flat-square&logo=github" alt="GitHub Stars"/>
  </a>
</p>

<p align="center">
  <strong>If you find this project useful, please consider giving it a ⭐ on GitHub!</strong>
</p>

---

## BLUF (Bottom Line Up Front)

ScreenBloom is an AI-powered mobile application designed to help users reclaim their focus and cultivate a healthier digital life. It intelligently replaces compulsive social media scrolling with personalized goal tracking, mindfulness exercises, and custom app blockers to foster mindful technology use.

## Table of Contents

- [Architecture](#architecture)
- [🤖 AI Agent Directives](#-ai-agent-directives)
- [Development Standards](#development-standards)
- [Features](#features)
- [Installation & Setup](#installation--setup)
- [Usage](#usage)
- [Contributing](#contributing)
- [Security](#security)
- [License](#license)

## Architecture

The app is built following a **Feature-Sliced Design (FSD)** architecture for scalability and maintainability, deployed using **Expo Application Services (EAS)**.


ScreenBloom/
├── .github/                 # GitHub Workflows, Templates, etc.
├── src/
│   ├── app/                 # App Entry Point (App.tsx, app.json)
│   ├── entities/            # Business logic (e.g., User, Goal)
│   ├── features/            # Feature-specific UI and logic
│   │   ├── auth/            # Authentication flow
│   │   ├── goals/           # Goal tracking
│   │   ├── blocker/         # App blocking logic
│   │   └── mindfulness/     # Mindfulness games
│   ├── pages/               # Screen components
│   ├── shared/              # Cross-cutting concerns (UI kit, lib, api)
│   └── processes/           # Global orchestration (e.g., startup, error handling)
├── assets/                  # Static assets (images, fonts)
├── __tests__/               # Jest/Pitest test suites
└── package.json


## 🤖 AI Agent Directives

<details>
<summary>Click to expand AI Directives</summary>

### Tech Stack Definition
- **Platform:** Mobile (iOS/Android)
- **Language:** TypeScript (Strict)
- **Framework:** React Native with Expo SDK
- **State Management:** Zustand
- **Navigation:** Expo Router (File-based)
- **Styling:** StyleSheet + Tamagui for theme consistency
- **Testing:** Jest, React Native Testing Library (RNTL)
- **Linting/Formatting:** ESLint (Airbnb config), Prettier
- **CI/CD:** GitHub Actions (EAS Build & Submit)

### Architectural Patterns
- **Architecture:** Feature-Sliced Design (FSD)
- **Principles:** SOLID, DRY, YAGNI, You Aren't Gonna Need It.
- **Design System:** Component-driven UI in `shared/ui`.
- **Data Flow:** Unidirectional data flow via Zustand stores.
- **Error Boundaries:** Implemented at feature-level to prevent crashes.

### Verification Commands
- **Lint:**
  bash
  npm run lint
  
- **Format:**
  bash
  npm run format
  
- **Type Check:**
  bash
  npm run type-check
  
- **Run Tests:**
  bash
  npm run test
  
- **Start Development Server:**
  bash
  npm run start
  

</details>

## Development Standards

### Setup

1.  **Clone the repository:**
    bash
    git clone https://github.com/chirag127/ScreenBloom-Social-Media-Detox-Mobile-App.git
    cd ScreenBloom-Social-Media-Detox-Mobile-App
    
2.  **Install dependencies:**
    bash
    npm install
    

### Scripts

| Script | Command | Description |
| :--- | :--- | :--- |
| `start` | `npx expo start` | Starts the Metro bundler and development server. |
| `android` | `npx expo start --android` | Runs the app on a connected Android device/emulator. |
| `ios` | `npx expo start --ios` | Runs the app on a connected iOS device/simulator. |
| `build:android`| `eas build --platform android` | Creates a production build for Android. |
| `build:ios` | `eas build --platform ios` | Creates a production build for iOS. |
| `lint` | `eslint . --ext .js,.jsx,.ts,.tsx` | Lints the codebase for style and error issues. |
| `format` | `prettier --write .` | Formats all files to match project standards. |

### Principles
- **SOLID:** Adhere to the five principles for robust object-oriented design.
- **DRY:** Do not repeat yourself; abstract reusable logic into libraries or components.
- **YAGNI:** Avoid implementing functionality until it is necessary.

## Features

- **🎯 Personalized Goal Tracking:** Set, monitor, and achieve personal goals, replacing mindless scrolling with productive habits.
- **🧘 Mindfulness Games:** Engage in short, interactive exercises designed to reduce anxiety and improve focus.
- **🚫 Custom App Blockers:** Create powerful, flexible rules to block distracting apps during specific times or after reaching usage limits.
- **📊 Usage Analytics:** Visualize your digital habits with clear, insightful charts and statistics.
- **🔔 Gentle Nudges:** Receive intelligent, non-intrusive notifications encouraging you to stay on track.

## Installation & Setup

> **Note:** ScreenBloom is currently in development. A public beta will be available on the TestFlight and Google Play Console soon.

1.  Ensure you have [Node.js](https://nodejs.org/) (v18 or higher) installed.
2.  Install the Expo Go app on your iOS or Android device.
3.  Clone the repo and install dependencies as described in the [Development Standards](#setup).
4.  Run `npm run start` and scan the QR code with the Expo Go app.

## Usage

Upon launching ScreenBloom, you'll be guided through a simple onboarding process to set your current wellness goals. The dashboard provides a clear overview of your progress, blocked apps, and mindfulness tools.

## Contributing

We welcome contributions! Please read our [`CONTRIBUTING.md`](CONTRIBUTING.md) guide for details on our code of conduct and the process for submitting pull requests. All contributions must adhere to our linting and testing standards.

## Security

We take security seriously. Please review our [`SECURITY.md`](SECURITY.md) for our policy and how to report vulnerabilities responsibly.

## License

This project is licensed under the Creative Commons Attribution-NonCommercial 4.0 International License. See the [`LICENSE`](LICENSE) file for details.
