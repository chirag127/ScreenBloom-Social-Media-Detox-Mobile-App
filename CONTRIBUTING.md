# Contributing to ScreenBloom-Social-Media-Detox-Mobile-App

## Table of Contents
- [Introduction](#introduction)
- [Getting Started](#getting-started)
- [Development Workflow](#development-workflow)
- [Testing](#testing)
- [Linting & Formatting](#linting--formatting)
- [Commit Message Guidelines](#commit-message-guidelines)
- [Pull Request Process](#pull-request-process)
- [Issue Reporting](#issue-reporting)
- [Code of Conduct](#code-of-conduct)
- [License](#license)

---

### Introduction
Thank you for your interest in improving **ScreenBloom – Social Media Detox Mobile App**! This guide outlines how you can contribute effectively while keeping the project high‑velocity, zero‑defect, and future‑proof.

---

### Getting Started
1. **Fork the repository** on GitHub.
2. **Clone your fork**:
   bash
   git clone https://github.com/chirag127/ScreenBloom-Social-Media-Detox-Mobile-App.git
   cd ScreenBloom-Social-Media-Detox-Mobile-App
   
3. **Install Node.js (v20+)** and a package manager (`npm` or `pnpm`).
4. **Install dependencies**:
   bash
   npm ci   # uses the lockfile for reproducible installs
   
5. **Configure environment variables**:
   bash
   cp .env.example .env
   # edit .env if you need custom values
   
6. **Run the app** with Expo:
   bash
   npx expo start
   
   This will launch the Metro bundler. Scan the QR code with the Expo Go app on your device or run an emulator.

---

### Development Workflow
| Step | Command | Description |
|------|---------|-------------|
| **Start** | `npx expo start` | Launch development server |
| **Run iOS** | `npx expo run:ios` | Build & run on iOS simulator |
| **Run Android** | `npx expo run:android` | Build & run on Android emulator |
| **Lint** | `npm run lint` | Run Biome linting |
| **Format** | `npm run format` | Auto‑format code with Biome |
| **Test** | `npm test` | Execute Vitest unit tests |
| **E2E** | `npm run test:e2e` | Execute Playwright end‑to‑end tests |

---

### Testing
- **Unit Tests**: Located in `tests/unit/`. Run with `npm test`.
- **End‑to‑End Tests**: Located in `tests/e2e/`. Run with `npm run test:e2e`.
- All tests must pass before a PR can be merged. CI will enforce this via GitHub Actions.

---

### Linting & Formatting
We use **Biome** for both linting and auto‑formatting.
- Lint: `npm run lint`
- Fix lint issues: `npm run lint -- --fix`
- Format: `npm run format`
- Check formatting: `npm run format -- --check`
Any lint or formatting errors will cause the CI pipeline to fail.

---

### Commit Message Guidelines
Follow **Conventional Commits** to keep the history readable and enable automated changelog generation.

<type>(<scope>): <subject>

<body> (optional)

<footer> (optional, e.g., "BREAKING CHANGE:")

**Types**: `feat`, `fix`, `docs`, `style`, `refactor`, `test`, `chore`, `perf`, `ci`.
**Scope**: Directory or feature name, e.g., `ui`, `auth`, `tracker`.

---

### Pull Request Process
1. **Create a feature branch** from `main`:
   bash
   git checkout -b feat/<short-description>
   
2. **Commit** using the Conventional Commits format.
3. **Push** the branch and **open a PR** against `main`.
4. **Link** the PR to an existing issue (or create a new one) using the `#issue-number` reference.
5. Ensure **all checks** (tests, lint, format) pass.
6. Request reviews from at least one maintainer.
7. Once approved, **squash‑merge** the PR to keep a clean history.

---

### Issue Reporting
- Use the provided issue templates in `.github/ISSUE_TEMPLATE/`.
- Include a clear title, reproduction steps, expected vs. actual behavior, and environment details (OS, device, Expo version).
- Tag the issue with appropriate labels (`bug`, `enhancement`, `question`).

---

### Code of Conduct
We expect all contributors to follow the project's [Code of Conduct](https://github.com/chirag127/ScreenBloom-Social-Media-Detox-Mobile-App/blob/main/CODE_OF_CONDUCT.md).

---

### License
By contributing, you agree that your contributions are licensed under the **CC BY-NC 4.0** license, matching the repository's license.

---

*Happy coding! 🎉*