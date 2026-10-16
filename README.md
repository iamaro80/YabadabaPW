# YabadabaPW 🔐

**YabadabaPW** is a modern, client-side, zero-tracking Material Design 3 (M3) Password Generator & Vault built as a fast, self-contained Single Page Application (SPA).

![Material Design 3](https://img.shields.io/badge/Design-Material%20Design%203-6750A4)
![Security-Client%20Side](https://img.shields.io/badge/Security-Client--Side%20Web%20Crypto-emerald)
![License](https://img.shields.io/badge/License-MIT-blue)

---

## ✨ Features

- **True Cryptographic Entropy**: Generates secure random sequences using the browser's native `window.crypto.getRandomValues()`.
- **Material Design 3 Interface**: Expressive M3 surfaces, rounded containers, dynamic elevation, and clean typography.
- **Dark & Light Mode**: Seamless theme switching with automatic system preference detection and `localStorage` persistence.
- **Password Entropy & Strength Meter**: Real-time entropy calculation (in bits) with dynamic strength tier indicators (*Weak*, *Fair*, *Strong*, *Very Strong*).
- **Flexible Character Sets**:
  - Uppercase letters (`A-Z`)
  - Lowercase letters (`a-z`)
  - Numbers (`0-9`)
  - Default & custom symbol sets (e.g. `!@#$%^&*...` or user-defined symbols)
- **Advanced Rules**:
  - **Exclude Ambiguous Characters**: Eliminates visually confusing characters like `0`, `O`, `o`, `1`, `l`, `I`, `|`, `;`, `:`.
  - **Leading Character Control**: Enforce whether passwords begin with an uppercase letter, lowercase letter, number, symbol, or random choice.
  - **Quick Length Presets**: Instant length chips (`12`, `16`, `24`, `32`) plus a continuous slider (`8`–`64` characters).
- **Persistent Vault Storage**:
  - Save generated passwords directly to local browser storage (`localStorage`).
  - Copy individual saved passwords with instant feedback (`✓ Copied`).
  - Delete individual entries or clear the entire vault.
  - Export saved vault passwords to `.txt`.
- **Single Page Application (SPA)**: Zero build step required; runs directly in any browser or static web host.

---

## 🚀 Getting Started

Simply open `index.html` or `yabadabapw.html` in any modern web browser, or serve it with any lightweight HTTP server:

```bash
# Using Python
python3 -m http.server 8000

# Using Node.js
npx serve .
```

Then visit `http://localhost:8000` in your browser.

---

## 🔒 Privacy & Security

YabadabaPW generates all credentials strictly in-memory inside the client browser. No passwords, preferences, or telemetry data are ever transmitted across networks or logged to remote servers.

---

## 📄 License

MIT License.
