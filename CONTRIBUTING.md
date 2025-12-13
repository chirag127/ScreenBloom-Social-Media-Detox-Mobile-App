# Contributing to ScreenBloom-Social-Media-Detox-Mobile-App

Thank you for your interest in contributing to **ScreenBloom**, a React Native app designed to promote digital wellness. This guide will help you get started.

## 🚀 Getting Started

### Prerequisites

-   **Node.js**: Version `20.x` or later.
-   **npm**: Version `10.x` or later, or **yarn** version `1.22.x` or later.
-   **Expo CLI**: `npm install -g @expo/cli`
-   **A mobile device or emulator/simulator**: For testing.

### Setup

1.  **Fork and Clone the Repository**
    bash
    git clone https://github.com/chirag127/ScreenBloom-Social-Media-Detox-Mobile-App.git
    cd ScreenBloom-Social-Media-Detox-Mobile-App
    
2.  **Install Dependencies**
    bash
    npm install
    # or
    yarn install
    
3.  **Start the Development Server**
    bash
    npm start
    # or
    yarn start
    
    Follow the on-screen instructions to open the project in the Expo Go app on your device or to run it on an emulator/simulator.

## 🧰 Development Standards

### Code Style

-   We use **TypeScript**. Please write all new code in TypeScript.
-   Follow the **[Airbnb JavaScript Style Guide](https://airbnb.io/javascript/)** as a baseline.
-   We use **ESLint** and **Prettier** for code formatting and linting. A pre-commit hook is configured to run these automatically.
    bash
    npm run lint
    npm run format
    

### Architectural Principles

-   **Feature-First Structure**: Organize your code by features. Each feature should be a self-contained directory with its own components, screens, hooks, and state management.
-   **Reusable Components**: Build UI components in the `components/` directory. They should be generic and well-documented.
-   **State Management**: Use **Zustand** for global state management. Keep local state within components using React's `useState` and `useReducer`.
-   **API Calls**: Centralize API logic in a dedicated `services/` directory. Abstract platform-specific interactions (like app blocking) into a `modules/` directory with a unified interface.

### Git Commit Convention

We follow the [Conventional Commits](https://www.conventionalcommits.org/) specification.
-   `feat:`: A new feature.
-   `fix:`: A bug fix.
-   `docs:`: Documentation only changes.
-   `style:`: Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc).
-   `refactor:`: A code change that neither fixes a bug nor adds a feature.
-   `test:`: Adding missing tests or correcting existing tests.

**Example:**
bash
git commit -m "feat(goal-tracker): add progress chart component"


## 🧪 Testing

-   **Unit & Integration Tests**: We use **Jest** and **React Native Testing Library**.
    bash
    npm test
    
-   **E2E Tests**: We use **Detox** for end-to-end testing.
    bash
    npm run test:e2e
    
-   **Coverage**: Aim for high test coverage. New features should include corresponding tests. A check is in place to ensure coverage standards are met.

## 📤 Submitting a Pull Request

1.  **Create a Branch**: From the `main` branch, create a descriptive branch for your feature or bug fix.
    bash
    git checkout -b feature/your-feature-name
    
2.  **Make Your Changes**: Follow the development standards outlined above. Ensure your code is clean and well-documented.
3.  **Test Your Changes**: Run the full test suite and ensure all tests pass.
4.  **Commit Your Changes**: Use the conventional commit message format.
5.  **Push to Your Fork**:
    bash
    git push origin feature/your-feature-name
    
6.  **Open a Pull Request**:
    -   Go to the original repository on GitHub.
    -   Click "New Pull Request".
    -   Provide a clear and concise title and description for your PR. Reference any related issues using keywords like `closes #123`.

### PR Checklist

-   [ ] My code follows the style guidelines of this project.
-   [ ] I have performed a self-review of my own code.
-   [ ] I have commented my code, particularly in hard-to-understand areas.
-   [ ] I have made corresponding changes to the documentation.
-   [ ] My changes generate no new warnings.
-   [ ] I have added tests that prove my fix is effective or that my feature works.
-   [ ] New and existing unit tests pass locally with my changes.
-   [ ] Any dependent changes have been merged and published in downstream modules.

## 🐛 Reporting Bugs

If you find a bug, please open an issue using our [bug report template](https://github.com/chirag127/ScreenBloom-Social-Media-Detox-Mobile-App/blob/main/.github/ISSUE_TEMPLATE/bug_report.md). Provide as much detail as possible, including steps to reproduce, expected vs. actual behavior, and your environment (OS, app version, etc.).

## 💡 Suggesting Enhancements

We welcome ideas for new features and improvements. Please open an issue and use the `enhancement` label. Describe your idea, the problem it solves, and any potential implementation approaches.

## 📜 License

By contributing, you agree that your contributions will be licensed under the [Creative Commons Attribution-NonCommercial 4.0 International License](LICENSE).

## 🤝 Code of Conduct

This project adheres to a code of conduct. By participating, you are expected to uphold this code. Please be respectful, welcoming, and inclusive to all contributors.

Thank you for contributing to ScreenBloom! Your efforts help make digital wellness accessible to everyone. 🌱