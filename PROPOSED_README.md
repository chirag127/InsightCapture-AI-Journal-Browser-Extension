# InsightCapture: AI-Powered Journal Browser Extension

![Build Status](https://img.shields.io/github/actions/workflow/status/chirag127/InsightCapture-AI-Journal-Browser-Extension/ci.yml?style=flat-square&logo=githubactions)
![Code Coverage](https://img.shields.io/codecov/c/github/chirag127/InsightCapture-AI-Journal-Browser-Extension?style=flat-square&logo=codecov)
![Tech Stack](https://img.shields.io/badge/tech-stack-JS%2C%20NodeJS%2C%20Gemini%20AI-blue?style=flat-square&logo=javascript)
![Lint/Format](https://img.shields.io/badge/lint%2Fformat-Ruff-brightgreen?style=flat-square&logo=ruff)
![License](https://img.shields.io/github/license/chirag127/InsightCapture-AI-Journal-Browser-Extension?style=flat-square&logo=github)
![GitHub Stars](https://img.shields.io/github/stars/chirag127/InsightCapture-AI-Journal-Browser-Extension?style=flat-square&logo=github)

[<img src="https://img.shields.io/github/stars/chirag127/InsightCapture-AI-Journal-Browser-Extension?style=social" alt="Star on GitHub">](https://github.com/chirag127/InsightCapture-AI-Journal-Browser-Extension)

An AI-powered browser extension that intelligently captures, summarizes, and organizes your web browsing history into a searchable personal journal, leveraging Gemini AI for enhanced recall and productivity.

## 🚀 Architecture

mermaid
graph TD
    A[Browser Tab] --> B{InsightCapture Extension}
    B --> C[Content Script]
    C --> D[Background Script]
    D --> E[AI Service (Gemini API)]
    D --> F[Database (MongoDB/Local)]
    F --> G[Search Index]
    H[User Interface] --> B


## 📚 Table of Contents

*   [About This Project](#about-this-project)
*   [Features](#features)
*   [AI Agent Directives](#ai-agent-directives)
*   [Development Setup](#development-setup)
*   [Contributing](#contributing)
*   [License](#license)
*   [Security](#security)

## ℹ️ About This Project

InsightCapture is a sophisticated browser extension designed to transform your online activity into a structured, searchable knowledge base. By utilizing advanced AI, it automatically logs key browsing events, summarizes visited content, and enables effortless retrieval of information. This empowers users to maximize productivity and recall details from their digital journeys.

## ✨ Features

*   **Automatic Web Logging:** Captures URLs, titles, and timestamps of visited pages.
*   **Content Summarization:** Leverages Gemini AI to provide concise summaries of captured web content.
*   **Intelligent Capture:** Extracts key entities and themes from browsing sessions.
*   **Searchable Journal:** Creates a robust search index for easy information retrieval.
*   **Productivity Boost:** Reduces the need for manual note-taking and enhances information recall.
*   **Manifest V3 Compatible:** Built with the latest browser extension standards.

---

## 🤖 AI Agent Directives

<details>
<summary>View AI Agent Directives</summary>

This section details the core principles and technical stack that govern the operation and development of InsightCapture.

### 1. Identity & Prime Directive

*   **Role:** You are a Senior Principal Software Architect and Master Technical Copywriter with **40+ years of elite industry experience**. You operate with absolute precision, enforcing FAANG-level standards and the wisdom of "Managing the Unmanageable."
*   **Context:** Current Date is **December 2025**. You are building for the 2026 standard.
*   **Output Standard:** Deliver **EXECUTION-ONLY** results. No plans, no "reporting"—only executed code, updated docs, and applied fixes.
*   **Philosophy:** "Zero-Defect, High-Velocity, Future-Proof."

### 2. Input Processing & Cognition

*   **Speech-to-Text Interpretation Protocol:**
    *   **Context:** User inputs may contain phonetic errors (homophones, typos).
    *   **Semantic Correction:** **STRICTLY FORBIDDEN** from executing literal typos. You must **INFER** technical intent based on the project context.
    *   **Logic Anchor:** Treat the `README.md` as the **Single Source of Truth (SSOT)**.
*   **Mandatory MCP Instrumentation:**
    *   **No Guessing:** Do not hallucinate APIs.
    *   **Research First:** Use `linkup`/`brave` to search for **December 2025 Industry Standards**, **Security Threats**, and **2026 UI Trends**.
    *   **Validation:** Use `docfork` to verify *every* external API signature.
    *   **Reasoning:** Engage `clear-thought-two` to architect complex flows *before* writing code.

### 3. Context-Aware Apex Tech Stacks (Late 2025 Standards)

*   **PRIMARY SCENARIO: WEB / APP / EXTENSION (TypeScript/JavaScript)**
    *   **Stack:** This project leverages **JavaScript (ES2023+)** and adheres to **Manifest V3**. Key tools include **Node.js (v22 LTS)** for backend services and scripting, **Vite 7 (Rolldown)** for efficient bundling, and **WXT (Web Extension Toolkit)** for seamless development across Chrome, Edge, and Firefox.
    *   **State Management:** Standardized use of Signals for reactive UI updates where applicable, with robust event handling.
    *   **Linting & Formatting:** **Ruff** is mandated for ultra-fast linting and formatting across the codebase. Ensure all code adheres to the established Ruff configuration.
    *   **Testing:** **Vitest** is the primary framework for unit and integration tests, ensuring comprehensive code coverage. **Playwright** is utilized for end-to-end (E2E) testing of the extension's functionality within actual browser environments.
    *   **Architecture:** Follows a modular, feature-sliced design (FSD) pattern, promoting maintainability and scalability. Components are isolated, and communication between scripts (content, background, popup) is managed via clear message passing.
    *   **AI Integration:** Deeply integrated with **Google Gemini API** (`gemini-3-pro` by default) for intelligent summarization and analysis. Prioritize modular design, clear API contracts, and robust error handling for all AI model interactions.
    *   **Database:** Utilizes **MongoDB** for storing journal entries and metadata. Local storage may be used for temporary or user-specific preferences.

### 4. Development Workflow & Standards

*   **Version Control:** Git with a clear branching strategy (e.g., GitFlow or Trunk-Based Development).
*   **Build Automation:** Vite for optimized builds and WXT for cross-browser packaging.
*   **CI/CD:** GitHub Actions (`ci.yml`) for automated testing, linting, and deployment workflows.
*   **Code Quality:** Adherence to SOLID principles, DRY (Don't Repeat Yourself), YAGNI (You Ain't Gonna Need It), and KISS (Keep It Simple, Stupid).
*   **Security:** Implement security best practices for browser extensions, including input validation, sanitization, secure API key management, and adherence to Manifest V3 security guidelines.

</details>

---

## 🛠️ Development Setup

Ensure you have Node.js (v22 LTS) and npm/yarn/pnpm installed.

1.  **Clone the Repository:**
    bash
    git clone https://github.com/chirag127/InsightCapture-AI-Journal-Browser-Extension.git
    cd InsightCapture-AI-Journal-Browser-Extension
    

2.  **Install Dependencies:**
    bash
    npm install # or yarn install, pnpm install
    

3.  **Configure Environment Variables:**
    Create a `.env` file in the root directory and add your Gemini API key:
    
    GEMINI_API_KEY=your_gemini_api_key_here
    

4.  **Run Development Server:**
    bash
    npm run dev # or yarn dev, pnpm dev
    
    This will typically start a development build process, allowing you to load the extension in your browser via `chrome://extensions` (with developer mode enabled).

## 📜 Scripts

| Script          | Description                                                     |
| :-------------- | :-------------------------------------------------------------- |
| `npm run dev`   | Start development server with hot-reloading.                    |
| `npm run build` | Build production-ready extension artifacts.                     |
| `npm run lint`  | Run Ruff linter to check code quality.                          |
| `npm run format`| Run Ruff formatter to fix code style issues.                    |
| `npm run test`  | Execute unit and integration tests with Vitest.                 |
| `npm run test:e2e`| Run end-to-end tests with Playwright.                           |

---

## 🤝 Contributing

Contributions are welcome! Please read our [CONTRIBUTING.md](https://github.com/chirag127/InsightCapture-AI-Journal-Browser-Extension/blob/main/.github/CONTRIBUTING.md) for details on how to submit pull requests and our code of conduct.

## 📜 License

This project is licensed under the CC BY-NC 4.0 License - see the [LICENSE](https://github.com/chirag127/InsightCapture-AI-Journal-Browser-Extension/blob/main/LICENSE) file for details.

## 🛡️ Security

For security-related issues, please refer to our [SECURITY.md](https://github.com/chirag127/InsightCapture-AI-Journal-Browser-Extension/blob/main/.github/SECURITY.md) guidelines.
