# 🔒 Security Policy

This document outlines the security policy for the **InsightLog-AI-Assisted-Journal-Capture-Browser-Extension** project. We take the security of our users and their data with the utmost seriousness and are committed to maintaining a secure and reliable extension.

## 報告漏洞 (Reporting a Vulnerability)

We welcome and appreciate responsible disclosures from security researchers and the community. If you discover a security vulnerability within this project, please **do not open a public GitHub issue**. Instead, follow these steps:

1.  **Direct Email:** Send a detailed report to [security@chirag.dev](mailto:security@chirag.dev).
    *   **Subject:** `[SECURITY] InsightLog - Vulnerability Report - <Brief Summary>`
2.  **PGP Encryption (Optional but Recommended):** For sensitive information, we encourage encrypting your report using our PGP public key.
    
    -----BEGIN PGP PUBLIC KEY BLOCK-----
    Comment: This is a placeholder. Replace with an actual PGP public key for security@chirag.dev.

    -----END PGP PUBLIC KEY BLOCK-----
    
3.  **Details to Include:**
    *   **Type of vulnerability:** (e.g., XSS, CSRF, Injection, Data Leakage).
    *   **Affected versions:** Clearly state which versions or commits are affected.
    *   **Reproduction steps:** Provide clear, step-by-step instructions to reproduce the vulnerability.
    *   **Impact:** Describe the potential impact of the vulnerability.
    *   **Proof-of-concept (PoC):** Include any relevant code, screenshots, or network logs.
    *   **Your contact information (optional):** If you wish to be credited.

## 🤝 Our Commitment

Upon receiving a vulnerability report, we will:

1.  Acknowledge receipt of your report within **48 hours**.
2.  Investigate the issue thoroughly and assign it a priority level based on its severity and potential impact.
3.  Keep you informed of our progress throughout the remediation process.
4.  Publicly disclose the vulnerability and our fix, along with appropriate credit to the reporter (if desired), after the issue has been resolved and a new release has been deployed. We aim for a coordinated disclosure process.

## 🛡️ Best Practices for Contributors

All contributors are expected to adhere to secure coding practices:

*   **Input Validation:** Always validate and sanitize all user inputs on the client-side, especially before display or storage within the extension.
*   **Output Encoding:** Encode all output to prevent injection attacks (e.g., XSS).
*   **Principle of Least Privilege:** The extension and its components should operate with the minimum necessary permissions as defined in `manifest.json`.
*   **Dependency Management:** Regularly update third-party dependencies to mitigate known vulnerabilities. We leverage automated tools for this.
*   **Secure Storage:** Handle sensitive user data (e.g., personally identifiable information, API keys) with extreme care. Avoid storing highly sensitive, unencrypted data in `localStorage` or `IndexedDB`.
*   **Content Security Policy (CSP):** The extension's `manifest.json` **MUST** define a strict Content Security Policy to reduce the risk of XSS and data injection attacks.
*   **Minimal Permissions:** Request only the absolute minimum required permissions in `manifest.json`. Clearly justify each permission requested.
*   **Third-Party Libraries:** Vet all third-party libraries for known vulnerabilities and ensure they are actively maintained and reputable.

## 🚀 Supported Versions

The security team primarily focuses on the latest stable release of **InsightLog-AI-Assisted-Journal-Capture-Browser-Extension**. We encourage all users to upgrade to the latest version to ensure they benefit from the most recent security patches and features.

*   **Latest Stable Release:** Actively supported with security updates.
*   **Previous Major Releases:** May receive critical security updates on a case-by-case basis.

## 🌐 Project Links

*   **GitHub Repository:** [https://github.com/chirag127/InsightLog-AI-Assisted-Journal-Capture-Browser-Extension](https://github.com/chirag127/InsightLog-AI-Assisted-Journal-Capture-Browser-Extension)
*   **Contributing Guidelines:** [https://github.com/chirag127/InsightLog-AI-Assisted-Journal-Capture-Browser-Extension/blob/main/.github/CONTRIBUTING.md](https://github.com/chirag127/InsightLog-AI-Assisted-Journal-Capture-Browser-Extension/blob/main/.github/CONTRIBUTING.md)
*   **License:** [https://github.com/chirag127/InsightLog-AI-Assisted-Journal-Capture-Browser-Extension/blob/main/LICENSE](https://github.com/chirag127/InsightLog-AI-Assisted-Journal-Capture-Browser-Extension/blob/main/LICENSE)

Thank you for helping us keep **InsightLog** secure!