# 🌟 Contribution Guidelines for MindBloom Digital Wellbeing Mindfulness Mobile App

Welcome to the MindBloom project! We appreciate your interest in contributing to a platform dedicated to fostering healthier digital habits and digital wellbeing. As an Apex Authority project, contributions must adhere to the highest standards of quality, maintainability, and performance.

## 1. Core Philosophy & Compliance

All contributions are governed by the **Apex Technical Authority Principles**:

*   **Zero-Defect:** Aim for production-ready code. Thorough testing is mandatory.
*   **Future-Proof:** Favor modern, scalable patterns (e.g., FSD if applicable, or robust modularity in React Native).
*   **DRY & SOLID:** Adherence to the DRY (Don't Repeat Yourself) and SOLID principles is non-negotiable.

## 2. Development Workflow Prerequisites

Before submitting a Pull Request (PR), ensure your environment is configured according to the standards defined in the repository's root documentation.

1.  **Clone & Branch:** Fork the repository and create a feature branch named descriptively (e.g., `feat/new-meditation-timer` or `fix/crash-on-startup`).
    bash
    git clone https://github.com/chirag127/MindBloom-Digital-Wellbeing-Mindfulness-Mobile-App.git
    cd MindBloom-Digital-Wellbeing-Mindfulness-Mobile-App
    git checkout -b your-contribution-branch-name
    

2.  **Dependency Management (React Native/Expo):** Use the established package manager (`npm` or `yarn` as defined in the root setup) to install dependencies.
    bash
    # Example using npm, verify root package.json
    npm install
    

3.  **Code Quality Enforcement:** Run the local quality checks *before* committing. This ensures CI pipeline does not immediately fail due to style violations.
    bash
    # Linting & Formatting (Assuming Biome or ESLint/Prettier setup)
    npm run lint
    npm run format

    # Testing
    npm run test:unit
    # E2E tests (if applicable)
    npm run test:e2e
    

## 3. Submission Requirements (Pull Requests)

Every Pull Request **MUST** use the provided template (`.github/PULL_REQUEST_TEMPLATE.md`) and satisfy the following checks:

*   **Clear Description:** State *what* the change does and *why* it is necessary.
*   **Context Links:** Link to the relevant Issue (#) if one exists.
*   **Self-Verification:** Confirm you have run local tests (`npm run test`).
*   **No WIP:** Do not submit Work-In-Progress (WIP) PRs unless specifically requested for early feedback.

### Verification Checklist

If your PR modifies core logic, architecture, or introduces significant features, please confirm the following in your PR description:

*   [ ] Architectural adherence to Modular best practices (Feature-Sliced Design alignment, if applicable to React Native).
*   [ ] All new code paths are covered by unit or integration tests (Target Coverage: >85%).
*   [ ] External API interactions (e.g., date/time tracking, usage APIs) are resilient to network failures.
*   [ ] Performance impact assessed (especially for background usage tracking).

## 4. Issue Reporting

If you discover a bug or have an idea for a new feature:

1.  **Check Existing Issues:** Search existing open and closed issues to ensure it hasn't been reported or addressed.
2.  **Use Templates:** File a new issue using the provided template (`.github/ISSUE_TEMPLATE/bug_report.md`). Provide detailed steps to reproduce bugs.

## 5. Security Disclosure

We take digital wellbeing and data privacy seriously. If you discover a potential security vulnerability, please **DO NOT** open a public issue. Follow the guidelines outlined in our **Security Policy** (`.github/SECURITY.md`) for responsible disclosure.

--- 

*Thank you for helping us cultivate a more mindful digital landscape!*

**Project Repository:** `https://github.com/chirag127/MindBloom-Digital-Wellbeing-Mindfulness-Mobile-App`