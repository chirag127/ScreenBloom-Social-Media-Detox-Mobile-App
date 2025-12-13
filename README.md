# ScreenBloom Social Media Detox Mobile App

![ScreenBloom Banner](https://raw.githubusercontent.com/chirag127/ScreenBloom-Social-Media-Detox-Mobile-App/main/assets/banner.png)

[![Build Status](https://img.shields.io/github/actions/workflow/status/chirag127/ScreenBloom-Social-Media-Detox-Mobile-App/ci.yml?branch=main&style=flat-square)](https://github.com/chirag127/ScreenBloom-Social-Media-Detox-Mobile-App/actions)
[![Code Coverage](https://img.shields.io/codecov/c/github/chirag127/ScreenBloom-Social-Media-Detox-Mobile-App?style=flat-square)](https://app.codecov.io/gh/chirag127/ScreenBloom-Social-Media-Detox-Mobile-App)
[![Tech Stack](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&style=flat-square)](https://www.typescriptlang.org/)
[![Framework](https://img.shields.io/badge/React%20Native-61DAFB?logo=react&style=flat-square)](https://reactnative.dev/)
[![Lint](https://img.shields.io/badge/Biome-000?logo=biome&style=flat-square)](https://biomejs.dev/)
[![License](https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey?style=flat-square)](https://creativecommons.org/licenses/by-nc/4.0/)
[![Stars](https://img.shields.io/github/stars/chirag127/ScreenBloom-Social-Media-Detox-Mobile-App?style=flat-square)](https://github.com/chirag127/ScreenBloom-Social-Media-Detox-Mobile-App/stargazers)

**⭐ Star this repo if you find it useful!**

---

## TL;DR (BLUF)
**ScreenBloom empowers users to reclaim digital well‑being by replacing endless social‑media scrolling with goal‑tracking, mindfulness games, and custom app blockers—all inside a sleek React Native mobile app.**

---

## Architecture Overview
mermaid
flowchart TD
    A[User Interface] --> B[React Native (Expo) ]
    B --> C[State Management (Redux Toolkit)]
    C --> D[Feature Modules]
    D --> E[Local Persistence (AsyncStorage)]
    D --> F[Native Modules (App Blocker, Sensors)]
    D --> G[Analytics & Telemetry]


---

## Table of Contents
- [Getting Started](#getting-started)
- [Development Scripts](#development-scripts)
- [Project Structure](#project-structure)
- [AI Agent Directives](#ai-agent-directives)
- [Contributing](#contributing)
- [License](#license)

---

## Getting Started
bash
# Clone the repo
git clone https://github.com/chirag127/ScreenBloom-Social-Media-Detox-Mobile-App.git
cd ScreenBloom-Social-Media-Detox-Mobile-App

# Install dependencies (uses npm; Yarn works as well)
npm install

# Run the app in Expo Go (iOS/Android)
npx expo start


---

## Development Scripts
| Script | Description |
|--------|-------------|
| `npm run start` | Launch Expo development server |
| `npm run ios` | Build and run on iOS simulator |
| `npm run android` | Build and run on Android emulator |
| `npm run lint` | Run Biome linting and auto‑fix |
| `npm run test` | Execute Vitest unit tests |
| `npm run build` | Generate production bundle |

---

## Project Structure

ScreenBloom-Social-Media-Detox-Mobile-App/
├─ .github/                # CI/CD workflows & issue templates
├─ src/                    # Feature‑based source code
│   ├─ features/           # Each feature lives in its own folder
│   │   ├─ goalTracker/
│   │   ├─ mindfulnessGames/
│   │   └─ appBlocker/
│   ├─ components/        # Re‑usable UI components
│   ├─ store/              # Redux Toolkit store & slices
│   └─ utils/              # Helper functions
├─ assets/                 # Images, icons, splash screens
├─ tests/                  # Vitest test suites
├─ scripts/                # Build & maintenance scripts
├─ app.json                # Expo configuration
├─ biome.json              # Biome lint config
├─ package.json            # npm manifest
└─ tsconfig.json           # TypeScript config


---

## AI Agent Directives
<details>
<summary>Click to expand AI Agent Directives</summary>

**Tech Stack Definition**
- Language: **TypeScript** (strict mode enabled)
- Runtime: **React Native** with **Expo SDK 51**
- State Management: **Redux Toolkit** + **RTK Query**
- Lint/Format: **Biome** (configured for 100% rule coverage)
- Testing: **Vitest** (unit) + **React Native Testing Library** (component) + **Playwright** (E2E via Expo Web)
- CI/CD: GitHub Actions (Ubuntu‑latest)

**Architectural Patterns**
- **Feature‑Sliced Design** – each domain feature encapsulated with its own UI, state, and services.
- **SOLID** – interfaces for native modules, dependency injection via context providers.
- **DRY & YAGNI** – shared utilities live under `utils/`; avoid premature abstraction.

**Verification Commands**
bash
# Lint & auto‑fix
npm run lint

# Unit tests with coverage
npm run test -- --coverage

# End‑to‑end tests (Expo Web)
npx playwright test

# Full CI pipeline (locally)
act -j ci


**Self‑Healing Guidance**
- On lint failures, Biome will auto‑fix what it can; remaining issues are reported as GitHub Checks.
- Test flakiness triggers automatic re‑run up to 3 attempts via CI matrix.
- CI aborts on coverage < 90% and enforces the `codecov.yml` threshold.

</details>

---

## Contributing
Please read our [CONTRIBUTING.md](https://github.com/chirag127/ScreenBloom-Social-Media-Detox-Mobile-App/blob/main/CONTRIBUTING.md) for guidelines on how to submit pull requests, report bugs, and propose features.

---

## License
This project is licensed under the **Creative Commons Attribution‑NonCommercial 4.0 International (CC BY‑NC 4.0)**. See the `LICENSE` file for details.
