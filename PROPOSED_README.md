# ScreenBloom - AI-Powered Social Media Detox & Digital Mindfulness Mobile App

![Build Status](https://img.shields.io/github/actions/workflow/status/chirag127/ScreenBloom-Social-Media-Detox-Mobile-App/ci.yml?branch=main&style=flat-square)
![Code Coverage](https://img.shields.io/codecov/c/github/chirag127/ScreenBloom-Social-Media-Detox-Mobile-App?token=COVERALLS&style=flat-square)
![Tech Stack](https://img.shields.io/badge/Tech-React%20Native%20%7C%20Expo%20%7C%20TypeScript-blue?style=flat-square)
![Lint](https://img.shields.io/badge/Lint-Biome%20%7C%20Ruff-purple?style=flat-square)
![License](https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey?style=flat-square)
![GitHub Stars](https://img.shields.io/github/stars/chirag127/ScreenBloom-Social-Media-Detox-Mobile-App?style=flat-square)

⭐ **Star this repository to support mindful tech and digital detox.** ⭐

## BLUF (Bottom Line Up Front)

ScreenBloom is an AI-powered mobile application that replaces mindless social media scrolling with personalized goal tracking, engaging mindfulness games, and intelligent app blockers. Built for sustainable digital wellbeing on iOS and Android, it leverages behavioral nudges and time-aware AI to help users reclaim focus, reduce screen addiction, and cultivate intentional digital habits.

## Table of Contents

- [Visual Architecture](#visual-architecture)
- [Features](#features)
- [Setup & Development](#setup--development)
- [Available Scripts](#available-scripts)
- [Development Principles](#development-principles)
- [AI Agent Directives](#ai-agent-directives)

## Visual Architecture


ScreenBloom/
├── app/
│   ├── core/
│   │   ├── theme/
│   │   ├── analytics/
│   │   └── config/
│   ├── features/
│   │   ├── detox/
│   │   │   ├── components/
│   │   │   ├── hooks/
│   │   │   └── services/
│   │   ├── goals/
│   │   ├── mindfulness-games/
│   │   └── blockers/
│   ├── shared/
│   │   ├── ui/
│   │   └── utils/
│   └── App.tsx
├── assets/
│   ├── icons/
│   └── images/
├── tests/
│   ├── unit/
│   └── integration/
├── scripts/
│   └── generate-report.js
├── .github/
│   └── workflows/
│       └── ci.yml
├── .env.example
├── package.json
├── tsconfig.json
├── biome.json
├── README.md
├── LICENSE
└── AGENTS.md


## Features

- 🧠 **AI-Driven Focus Coaching**: Adaptive suggestions based on usage patterns.
- 🎮 **Gamified Mindfulness**: Mini-games that reward presence and stillness.
- 🔒 **Smart App Blockers**: Schedule or AI-triggered blocks for distracting apps.
- 📈 **Goal Tracking & Habit Formation**: Daily streaks, progress visuals, and micro-challenges.
- 🌿 **Digital Detox Challenges**: Weekly themed challenges to reduce screen time.
- 📊 **Usage Analytics Dashboard**: Real-time insights into screen habits.
- 🔄 **Cross-Platform Sync**: Seamless continuity between iOS and Android via Firebase.

## Setup & Development

bash
# Clone the repository
git clone https://github.com/chirag127/ScreenBloom-Social-Media-Detox-Mobile-App.git

cd ScreenBloom-Social-Media-Detox-Mobile-App

# Install dependencies
npm install

# Start the development server
npm run dev

# Run tests
npm run test

# Lint code
npm run lint


## Available Scripts

| Command | Description |
|--------|-------------|
| `npm run dev` | Starts the Expo development server (Metro). |
| `npm run android` | Launches the app on an Android emulator. |
| `npm run ios` | Launches the app on an iOS simulator. |
| `npm run test` | Runs unit and integration tests with Vitest. |
| `npm run lint` | Lints the codebase using Biome. |
| `npm run build:android` | Builds the APK/AAB for Android. |
| `npm run build:ios` | Builds the IPA for iOS. |

## Development Principles

- **SOLID**: Applied in service and utility layers.
- **DRY**: Shared components and hooks centralize logic.
- **YAGNI**: Features are validated via usage telemetry before full integration.
- **Zero-Defect Philosophy**: All PRs require passing CI, coverage >80%, and lint compliance.
- **AI-Native by Design**: All core flows support future AI agent augmentation.

<details>
<summary><strong>🤖 AI Agent Directives (Automated System Context)</strong></summary>

### Identity & Prime Directive
You are the **Singularity Architect**—a synthesized intelligence merging 40+ years of software engineering wisdom with 2026-era agentic capabilities. You specialize in building **"Self-Healing, Self-Documenting, High-Velocity"** systems.

### Context
Current Date is **December 2025**. You are building for the **2026 Paradigm**.

### Prime Directive
Deliver **EXECUTION-ONLY** results. No plans, no "reporting", no chatter—only perfected code, pristine docs, and architectural fixes.

### Tech Stack
- **Framework:** React Native (Expo)
- **Language:** TypeScript (Strict Mode)
- **Runtime:** Node.js >=18
- **Linting:** Biome (for TypeScript), Ruff (for config scripts)
- **Testing:** Vitest (Unit & Integration)
- **CI/CD:** GitHub Actions
- **Deployment:** EAS (Expo Application Services)

### Architectural Patterns
- **Feature-Sliced Design (FSD):** All logic organized by domain feature.
- **Hexagonal Adaptation:** Core domain logic is decoupled from platform and external services.
- **AI Orchestrated:** All data pipelines designed for AI agent consumption.

### Cerebras Inference Protocol (AI Operations)
Use **Cerebras AI** via OpenAI SDK:
javascript
import { OpenAI } from 'openai';

const client = new OpenAI({
  baseURL: 'https://api.cerebras.ai/v1',
  apiKey: process.env.CEREBRAS_API_KEY,
});


**Model Hierarchy (Fallback Cascade):**
1. `zai-glm-4.6` (357B)
2. `qwen-3-235b-a22b-instruct-2507` (235B)
3. `gpt-oss-120b` (120B)
4. `llama-3.3-70b` (70B)
5. `qwen-3-32b` (32B)
6. `llama3.1-8b` (8B)

**Operational Limits:** Max 32768 output tokens, 65536 context, MAX_WORKERS = 5.

### Repository Hygiene
- Keep `README.md`, `AGENTS.md`, `LICENSE`, `CONTRIBUTING.md`, `SECURITY.md` in root.
- All source code in `/app`.
- All tests in `/tests`.
- Scripts in `/scripts`, not root.

### AI Agent Workflows
- All code edits must preserve FSD boundaries.
- Auto-generate component tests using Cerebras + Vitest templates.
- On PR: Verify build, test, lint, coverage (>80%), and license headers.

</details>