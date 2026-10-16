# YabadabaPW 🔐
### Custom Rule-Compliant Strong Password Generator

**YabadabaPW** is a fast, client-side, zero-tracking Single Page Application designed to generate cryptographically strong passwords tailored to any website's specific policy rules (such as mandatory start characters, custom symbol constraints, and ambiguous-character filtering) while keeping an offline staging vault.

![Security-Client%20Side](https://img.shields.io/badge/Security-Client--Side%20Web%20Crypto-emerald)
![License](https://img.shields.io/badge/License-MIT-blue)

---

## 🎨 Four Handcrafted Themes

YabadabaPW includes a live header palette switcher supporting four distinct aesthetic profiles:

1. **❄️ Nordic Periwinkle (Palette 1)**:
   - Light-mode clean Scandinavian SaaS security aesthetic.
   - Primary: `#5B67A2` • Secondary: `#738BE7` • Canvas: `#F8F9FC` • Accents: `#BFC8EA` & `#7B86AA`
2. **🌅 Sunset Coral & Plum (Palette 2)**:
   - Rich twilight dark mode with energetic warm sunset tones.
   - Canvas: `#35284A` • Primary Coral: `#FB7D79` • Accents: `#FB9D7E`, `#F8CD9E` & `#F8D9C3`
3. **⚓️ Deep Navy & Sage Olive (Palette 6)**:
   - Executive defense dark mode combining oceanic depth with organic sage.
   - Canvas: `#040A1B` • Navy: `#335495` • Accents: `#91A471`, `#668BC4` & `#A5BECF`
4. **🌱 Cyber Lime & Slate Navy**:
   - High-voltage modern organic tech aesthetic.
   - Primary: `#82CC00` • Text & Headers: `#283B51` • Canvas: `#FCFEF9` • Cards: `#EAF5D2` • Accents: `#ADD96A` & `#81A76A`

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
