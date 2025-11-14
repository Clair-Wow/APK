# Azeroth Pet Keeper (APK)
*A World of Warcraft Retail addon for managing and summoning vanity pets.*

---

## 🐾 Overview
Azeroth Pet Keeper (APK) keeps a companion pet by your side without needing to open the Pet Journal all the time.  
It can automatically summon pets on login or after dismounting, summon manually with a button or minimap click, and maintain a clean favorites/blacklist system.

This version is built for **World of Warcraft Retail** (The War Within era) and uses **Interface 110000**.

The zone-based summoning system has been removed in this release for reliability, and a new anti-repeat system has been added to avoid summoning the same pet repeatedly.

---

## ✨ Features

- **Auto-Summon Pets**
  - Summon on login and/or after dismount
  - Optional indoors/outdoors/raid filtering

- **Favorites & Blacklist**
  - Mark pets as Favorites
  - Blacklist any pets you never want summoned

- **Smarter Random Summoning**
  - Choose from Any, Flying, or Non-Flying pets
  - Anti-repeat buffer prevents streaks by excluding the last 10 summoned pets
  - `/apk last` explicitly re-summons the previously summoned pet

- **Summon Counters**
  - Tracks how many times each pet has been summoned
  - Visible in the Pet Manager window

- **Blizzard-Style UI**
  - Options window using Blizzard frame templates
  - Scrollable, scale-aware layout
  - Dedicated Pet Manager window

- **Minimap Button**
  - Left-click: Summon pet
  - Right-click: Open Options
  - Drag to reposition around the minimap (button sits just outside the edge)
  - Tooltip shows the currently summoned pet

---

## 💬 Slash Commands

| Command | Description |
|--------|-------------|
| `/apk` | Summon a random pet |
| `/apk last` | Re-summon your last used pet |
| `/apk options` | Open the Options window |
| `/apk manager` | Open the Pet Manager |
| `/apk minimap show` | Show the minimap button |
| `/apk minimap hide` | Hide the minimap button |
| `/apk minimap reset` | Reset minimap button position |

> **Note:** Zone-based commands have been removed in this Retail build.

---

3. Restart WoW or run `/reload`.
4. Enable **Azeroth Pet Keeper** in the AddOns menu.

---

## 🧭 Compatibility

- **Retail only (Interface 110000)**
- Not designed or tested for Classic-era or MoP-Classic clients

---

## 🧰 Technical Details

- **Addon folder:** `Interface/AddOns/APK`
- **Interface:** `110000`
- **Saved Variables:** `APKDB`
- **Files:**
- `APK.lua` — Core logic (summoning, rules, slash commands)
- `APK_UI.lua` — Options panel, Pet Manager, minimap button
- `APK.toc` — Metadata and file manifest

- **Dependencies:** None (pure Blizzard API)

---

## 🧾 Changelog

See the full version history in  
[CHANGELOG.md](./CHANGELOG.md)

Highlights from the most recent release:
- Zone system removed (for now) due to incorrect pet selection cases
- Anti-repeat summoning logic added (prevents streaks)
- `/apk last` is now the only way to re-summon the previous pet on demand
- UI improvements in Options and Pet Manager
- Various performance and stability fixes

---

## 📜 License

MIT License — free for personal and commercial use.  
Credit **L. Clair** if redistributing or forking.

---

## ❤️ Acknowledgments

Thanks to the WoW addon community and everyone who still enjoys having their little digital companions by their side.
