# 🎮 EnzoCord Discord Gaming Badges Maxer

**Creator & Developer**: **Omar ELSabbagh (EnzoCord)**  
**All Rights Reserved © 2026 EnzoCord**

---

An automated, military-grade protected application built with **Node.js (ES Modules)**, featuring an interactive CLI console hub, real-time keyboard controls, and an advanced dual-detection spoofing engine to maximize new Discord profile gaming badges to Tier 10:

1. 🏆 **Game Variety Badge** (Play up to 100 verified unique Discord games).
2. ⏱️ **Game Time Badge** (Accumulate thousands of hours of gameplay towards 5,000 hrs max tier).
3. 📺 **Streaming Badge** (Broadcast gaming presence via Twitch/Discord activity).

---

## 🌟 Key Features

- 🕹️ **Interactive Console Hub**:
  - Full CLI interface allowing 100% control directly from the terminal without ever opening or editing `.env` or config files manually.
  - Interactive token configuration, rotation duration timer, stream settings, and spoofer controls.
- ⚡ **Live Farming Hotkeys**:
  - `[S]`: Skip current game instantly and transition to next title in queue.
  - `[P]`: Pause or resume rotation timer on the fly.
  - `[T]`: Toggle Streaming presence activity on/off in real-time.
  - `[M]` or `[Q]`: Save state and return to Main Menu cleanly.
  - `[Ctrl + C]`: Safe graceful shutdown with zero progress loss.
- 🛡️ **Military-Grade Obfuscation & Anti-Tamper Engine**:
  - Multi-layered code protection (Control Flow Flattening, RC4/Base64 string encryption, dead code injection, and self-defending mechanisms).
  - Built-in tamper-proof integrity checks protecting `EnzoCord - Omar ELSabbagh` attribution from modification or deobfuscation.
- 🎮 **Dual-Detection Spoofing Engine**:
  1. **Direct Gateway WebSocket**: Simulates official Discord desktop client with rich presence activity payloads (`timestamps.start`, `application_id`, and streaming status).
  2. **Local Windows Process Spoofer**: Detaches lightweight background processes (0% CPU, 3.5 KB) mirroring game executables (`cs2.exe`, `overwatch.exe`, etc.) so the official Discord desktop client detects active gameplay natively.
- 💾 **Smart Queue & Auto-Resume**:
  - Automatic progress tracking in `data/progress.json`. Safely resume right where you left off.

---

## 🚀 Installation & Usage

### 1. Install Dependencies
Ensure [Node.js](https://nodejs.org/) (v18 or newer) is installed, then run:
```bash
npm install
```

### 2. Start the Application
```bash
npm start
```
The EnzoCord interactive console will launch immediately, allowing you to configure your token, settings, or start badges farming directly.

---

## 🛡️ Build Protected Production Release

To compile and obfuscate the entire codebase into a tamper-proof distribution:
```bash
npm run build
```
*(Or select option `[6]` from the interactive console menu).*

To run the obfuscated release in `./dist/`:
```bash
npm run start:dist
```

---

## ⌨️ Live Keyboard Controls

| Key | Action |
| :---: | :--- |
| `S` | Skip current game immediately and play the next one |
| `P` | Pause / Resume the rotation timer |
| `T` | Toggle Streaming activity mode |
| `M` / `Q` | Save state and return to Main Control Hub |
| `Ctrl + C` | Safe shutdown with progress saved |

---

## 👑 Copyright & Attribution
- **Author**: Omar ELSabbagh
- **Brand**: EnzoCord
- **Copyright (c) 2026 EnzoCord - Omar ELSabbagh. All Rights Reserved.**
