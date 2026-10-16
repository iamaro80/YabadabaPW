# YabadabaPW 🔐
### Custom Rule-Compliant Strong Password Generator

**YabadabaPW** is a fast, client-side, zero-tracking Single Page Application designed to generate cryptographically strong passwords tailored to any website's specific policy rules (such as mandatory start characters, custom symbol constraints, and ambiguous-character filtering) while keeping an offline staging vault.

![Security-Client%20Side](https://img.shields.io/badge/Security-Client--Side%20Web%20Crypto-emerald)
![Design-Colorion%20566](https://img.shields.io/badge/Design-Colorion%20%23566-363671)
![License](https://img.shields.io/badge/License-MIT-blue)

---

## 🎨 Available Design Profiles

YabadabaPW includes a live header theme switcher supporting two refined profiles:

1. **🎨 Indigo Rose (Colorion #566)**:
   - Modern, editorial high-contrast security theme.
   - Deep Indigo (`#363671`), Watermelon Rose CTA (`#EE537C`), Seafoam Mint (`#8FC9BF`), and Cloud Slate canvas (`#F8F9FD`).
2. **⚡️ Electric Canary & Emerald (Extracted Theme)**:
   - High-visibility security aesthetic extracted directly from clean mobile-grade credentials UI.
   - Canary Yellow CTA (`#FEEA2D`), Electric Blue accents (`#1670EF`), Emerald Green border (`#38B174`), Mint pill (`#E7F4E3` / text `#40864D`), and crisp Charcoal borders (`#2F2F2F`).

---

## 🎯 What Makes YabadabaPW Different?

Many websites and enterprise portals enforce quirky, strict password requirements (e.g. *"must start with a letter"*, *"only allowed symbols: #@$"*, *"no ambiguous characters"*). Generic password generators often fail these rules, causing repeated signup frustration. 

**YabadabaPW** gives you precise policy controls without compromising cryptographic randomness:

- **Quick Profiles**: Instant 1-click profiles for *Standard 16*, *URL-Safe 20*, *High Security 32*, and *PIN (6 Digits)*.
- **Custom Allowed Symbols**: Limit symbols to the exact characters approved by your service (e.g. `#@$`), or use standard comprehensive punctuation.
- **Leading Character Rules**: Force passwords to start with an uppercase letter, lowercase letter, number, or symbol to satisfy legacy authentication systems.
- **Ambiguous Character Filter**: Exclude visually confusing characters (`0`, `O`, `o`, `1`, `l`, `I`, `|`, `;`, `:`) to ensure trouble-free manual typing.
- **True Cryptographic Entropy**: Relies entirely on the native Web Crypto API (`window.crypto.getRandomValues()`) with independent Fisher-Yates array shuffling.
- **Real-Time Entropy Meter**: Calculates mathematical entropy in bits with real-time feedback (*Weak*, *Fair*, *Strong*, *Very Strong*).
- **Offline Staging Vault**: Temporarily store, label, copy, and export `.txt` credential sets stored safely in browser `localStorage`.
- **Zero Network Transmission**: 100% client-side; no credentials, data, or telemetry ever leave your device.

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

YabadabaPW generates all credentials strictly in-memory inside the client browser. No passwords, preferences, or telemetry data are ever transmitted across networks or logged on remote servers.

---

## 📄 License

MIT License.
