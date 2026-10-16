# YabadabaPW 🔐
### Custom Rule-Compliant Strong Password Generator

**YabadabaPW** is a fast, client-side, zero-tracking Single Page Application designed to generate cryptographically strong passwords tailored to any website's specific policy rules (such as mandatory start characters, custom symbol constraints, and ambiguous-character filtering) while keeping an offline staging vault.

![Design](https://img.shields.io/badge/Design-Champagne%20%26%20Obsidian-262220)
![Security-Client%20Side](https://img.shields.io/badge/Security-Client--Side%20Web%20Crypto-emerald)
![License](https://img.shields.io/badge/License-MIT-blue)

---

## 🏛 Aesthetic: Champagne Beige & Obsidian Black

Designed around soft tones, bold contrasts, and architectural tactile surfaces:
- **Champagne Beige (Light Mode)**: Warm cashmere silk canvas, travertine cards, and obsidian typography.
- **Obsidian Black (Dark Mode)**: Velvety volcanic basalt, dark sculpted cards, and champagne silk text.
- **Editorial Typography**: Cormorant Garamond display serif paired with Plus Jakarta Sans and JetBrains Mono.

---

## 🎯 What Makes YabadabaPW Different?

Many websites and enterprise portals enforce quirky, strict password requirements (e.g. *"must start with a letter"*, *"only allowed symbols: #@$"*, *"no ambiguous characters"*). Generic password generators often fail these rules, causing repeated signup frustration. 

**YabadabaPW** gives you precise policy controls without compromising cryptographic randomness:

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
