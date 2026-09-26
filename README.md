# 🦇 ENZOCORD DISCORD GAMING BADGES MAXER

<p align="center">
  <img src="https://img.shields.io/badge/Author-Omar%20ELSabbagh-00f0ff?style=for-the-badge&logo=discord&logoColor=white" alt="Author" />
  <img src="https://img.shields.io/badge/Brand-EnzoCord-7928ca?style=for-the-badge" alt="Brand" />
  <img src="https://img.shields.io/badge/Node.js-%3E%3D18.0.0-00dfa2?style=for-the-badge&logo=node.js&logoColor=white" alt="Node" />
  <img src="https://img.shields.io/badge/Security-Military--Grade%20Obfuscated-ff0055?style=for-the-badge&logo=security&logoColor=white" alt="Security" />
  <img src="https://img.shields.io/badge/Status-Undetected%20%26%20Safe-brightgreen?style=for-the-badge" alt="Status" />
</p>

```
                  /|       |\
                 / |       | \
                /  |  ___  |  \
               |   | /   \ |   |
               |   | | O | |   |
                \   \| _ |/   /
                 \   \___/   /
             _____|         |_____
            /                     \
           |   ENZOCORD BADGES     |
            \_____________________/
```

> **Automated Dual-Detection Tool to Maximize All Discord Profile Gaming Badges to Tier 10**  
> **Engineered by Omar ELSabbagh (EnzoCord)**  
> **Copyright © 2026 EnzoCord. All Rights Reserved.**

---

## ⚡ Super-Fast Quick Start (Zero Config Required)

You do **NOT** need to edit or configure any `.env` files manually. EnzoCord features an **interactive Zero-Config smart boot**:
1. Clone the repository
2. Run `npm start`
3. If no token is detected, EnzoCord **prompts you directly in the terminal** to paste your Discord token, securely writes it to `.env`, and offers to start farming badges immediately!

### 💻 Commands

```bash
# 1. Clone the repository
git clone https://github.com/Omar-dv/GameBadgeMaxer.git
cd GameBadgeMaxer

# 2. Install dependencies
npm install

# 3. Launch EnzoCord
npm start
```

That's it! The tool will take care of everything automatically.

---

## 🔑 How to Get Your Discord Token (15-Second Guide)

Your token is required so EnzoCord can authenticate with the official Discord Gateway and register verified game presence payloads.

1. Open **Discord** in your web browser (Chrome, Brave, Edge, Firefox) or desktop client.
2. Press `Ctrl + Shift + I` (or `F12`) to open **Developer Tools**.
3. Navigate to the **Network** tab.
4. In the filter box at the top, type `/api`.
5. Click on any network request that appears (such as `science`, `messages`, or `users/@me`).
6. Look under **Request Headers** on the right side and find `authorization`.
7. Copy the entire token value and paste it when EnzoCord prompts you in the terminal.

> 🔒 **Security Notice**: Your token is stored **locally on your machine only** inside `.env`. It is never uploaded, shared, or transmitted anywhere other than the official encrypted Discord Gateway WebSocket (`wss://gateway.discord.gg`).

---

## 🏆 Badges Tiers & Capabilities

EnzoCord is designed to max out all three gaming profile badges introduced by Discord:

| Badge | Max Target Tier | How EnzoCord Handles It |
| :--- | :---: | :--- |
| 🎮 **Game Variety Badge** | **Tier 10** (100 Unique Games) | Rotates through verified Discord-detectable games automatically. Tracks played games in `data/progress.json` to prevent duplicates. |
| ⏱️ **Game Time Badge** | **Tier 10** (5,000 Total Hours) | Continuous 24/7 background session spoofing with real-time timestamps and automatic progress saving every 60 seconds. |
| 📺 **Streaming Presence** | **Active Broadcast** | Spoofs Twitch / YouTube stream activity with customizable stream titles displayed prominently on your profile. |

---

## 🎮 Interactive Live Dashboard & Hotkeys

While farming is active, EnzoCord provides an ASCII dashboard and **instant keyboard hotkeys** (no need to press Enter):

```
  ╔══════════════════════════════════════════════════════════════════╗
  ║                      ENZOCORD LIVE DASHBOARD                     ║
  ╚══════════════════════════════════════════════════════════════════╝
    Account      : EnzoUser#0001 (Online)
    Active Game  : Counter-Strike 2
    Spoofer      : DETACHED ACTIVE (cs2.exe) [0% CPU]
    Stream       : 🔴 LIVE | twitch.tv/discord
    Progress     : [████████████████░░░░] 74% (07:45 remaining)
    Variety      : 38/100 Games [Tier 4]
    Total Time   : 142h 30m | Streamed: 95h 15m
  ──────────────────────────────────────────────────────────────────
   [S] Skip Game   [P] Pause/Resume   [T] Toggle Stream   [M] Menu   [X] Exit
```

### ⌨️ Hotkey Controls

| Hotkey | Description |
| :---: | :--- |
| `[S]` | **Skip Game**: Marks the current game as completed and instantly transitions to the next game in the queue. |
| `[P]` | **Pause / Resume**: Freezes or unfreezes the rotation timer without losing elapsed session time. |
| `[T]` | **Toggle Streaming**: Turns stream presence on or off on the fly. |
| `[M]` / `[Q]` | **Hub Menu**: Saves current progress safely and returns to the Main Control Hub. |
| `[X]` / `[Ctrl+C]` | **Safe Exit**: Flushes all progress to disk and closes background processes gracefully. |

---

## 🕹️ Main Control Hub Features

Running `npm start` gives you full control through an interactive CLI menu:

- **`[1] 🚀 Start Badges Farming`**: Begins automated rotation with live stats and hotkeys.
- **`[2] ⚙️ Settings & Configuration`**: Change rotation intervals, target game count, stream URLs, titles, and spoofer toggles directly from the console.
- **`[3] 📊 Badges & Progress Statistics`**: View full breakdown of your current variety tier, total playtime, cycle count, and list of unplayed games.
- **`[4] 🎮 Manual Game Selector`**: Pick and immediately spoof any specific game from Discord's verified database.
- **`[5] 🔄 Reset All Progress`**: Cleanly wipe progress to start fresh if needed.
- **`[0] 🚪 Exit Application`**: Safely shutdown.

---

## 🛡️ Dual-Detection Spoofing Architecture

Most tools only send raw gateway packets or simple status messages that fail to register on Discord's desktop detection layer. EnzoCord combines two synchronized engines:

1. **Direct Gateway Protocol Engine (`src/gateway.js`)**:
   - Maintains an authentic Discord Gateway WebSocket connection (`v9/v10`).
   - Dispatches full rich presence payloads (`timestamps.start`, `application_id`, `assets`, `details`, and `type 1` streaming presence).
2. **Local Windows Process Spoofer (`src/process_spoofer.js`)**:
   - Dynamically creates lightweight background processes mimicking genuine executable names (`cs2.exe`, `overwatch.exe`, `valorant.exe`).
   - Consumes **0% CPU and only 3.5 KB RAM**.
   - Causes the official Discord Desktop Client running on your PC to natively recognize the game as running.

---

## 🔒 Security & Anti-Tamper Notice

This release is protected by **EnzoCord Military-Grade Obfuscation Shield**:
- Control Flow Flattening & Dead Code Injection
- RC4 / Base64 Dynamic String Encryption
- Self-Defending Runtime Verification
- Embedded Anti-Tamper Copyright Assertion for **EnzoCord - Omar ELSabbagh**

Any unauthorized attempts to deobfuscate, modify, or strip developer credits will automatically terminate runtime execution.

---

## 👑 Credits & Author

- **Lead Developer**: **Omar ELSabbagh**
- **Brand**: **EnzoCord**
- **GitHub**: [@Omar-dv](https://github.com/Omar-dv)
- **Repository**: [Omar-dv/GameBadgeMaxer](https://github.com/Omar-dv/GameBadgeMaxer)
- **Copyright**: © 2026 **EnzoCord - Omar ELSabbagh**. All Rights Reserved.
