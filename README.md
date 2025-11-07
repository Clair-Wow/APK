# Azeroth Pet Keeper (APK)
*A World of Warcraft AddOn for managing and summoning vanity pets.*

---

## 🐾 Overview
**Azeroth Pet Keeper (APK)** is a modern, Blizzard-style addon that gives you full control over your companion pets.  
It can automatically summon, randomize, or favorite pets, while letting you blacklist the ones you’d rather keep in the kennel.

This addon was written from scratch for **Dragonflight / The War Within** and **Classic Mists of Pandaria**, with a native Blizzard UI look — no external libraries required.

---

## ✨ Features
- **Auto-Summon Pets**
  - On login and/or dismount  
  - Optional indoor/outdoor/raid conditions  
- **Favorites & Blacklist**
  - Mark pets you love or skip the ones you don’t  
- **Random Summoning**
  - Choose from *Any*, *Flying*, or *Non-Flying* pets  
- **Zone-Based Pet Sets**
  - Assign a unique set of pets per zone (`/apk zone add`)  
- **“Last Used” Recall**
  - Instantly resummon your previous companion (`/apk last`)  
- **Summon Counters**
  - Tracks how often each pet is summoned  
- **Graphical Interface**
  - Blizzard-styled windows for Options and Pet Manager  
  - Scrollable and UI-scale aware  
- **Minimap Button**
  - Left-click: Summon  
  - Right-click: Options  
  - Drag to reposition (radius sits just outside the minimap rim)  

---

## 🧭 Slash Commands
| Command | Description |
|----------|-------------|
| `/apk` | Summon a random pet |
| `/apk options` | Open options window |
| `/apk manager` | Open the Pet Manager |
| `/apk last` | Summon your last used pet |
| `/apk minimap show` / `hide` / `reset` | Control minimap button |
| `/apk zone on` / `off` / `add` / `clear` | Manage zone-based pets |

---

## 🪄 Installation
1. **Download** the latest release ZIP from GitHub or CurseForge.  
2. **Extract** the folder `APK` to your WoW AddOns directory:  
   - **Retail:** `_retail_/Interface/AddOns/APK`  
   - **Classic (MoP):** `_classic_mop_/Interface/AddOns/APK`  
3. **Restart WoW** and enable *Azeroth Pet Keeper* in the AddOns menu.

---

## 🧩 Technical Details
- **Addon Folder:** `Interface/AddOns/APK`
- **Saved Variables:** `APKDB`
- **Files:**
  - `APK.toc` — Manifest and metadata  
  - `APK.lua` — Core logic (summoning, data, slash commands)  
  - `APK_UI.lua` — Blizzard-styled interface (options, minimap, manager)  
- **Dependencies:** None (uses Blizzard API only)
- **Interface Version:** 110000

---

## ⚙️ Planned Enhancements
- Weighted random favorites  
- Zone-specific themes  
- Holiday pet rotations  
- Keybinding for “Summon Pet”  
- Export/import pet lists

---

## 📜 License
MIT License — free to use, modify, and share.  
Please credit **L Clair & ChatGPT** if redistributing or forking.

---

## ❤️ Acknowledgments
Special thanks to the **WoW API dev community** and all players who still care about their tiny virtual critters.

---


## Changelog
See [CHANGELOG.md](CHANGELOG.md) for version history.
