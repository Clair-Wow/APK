# Azeroth Pet Keeper — Changelog

---

## v1.3.0 — November 2025 (Retail)
**Smarter randomization and streamlined behavior.**

### 🔧 Major Changes
- **Zone System Removed (Retail):**  
  Temporarily removed zone-based pet sets to simplify behavior and avoid incorrect pet selections.  
  All summoning now works from your overall collection (with favorites/blacklist and filters).

- **Anti-Repeat Summoning:**  
  Added a recent-history buffer so the same pet isn’t summoned over and over.  
  The last 10 summoned pets are excluded from the random pool by default.

- **Removed “Prefer Last on Auto”:**  
  Auto-summon on login/dismount no longer re-summons the previous pet.  
  `/apk last` still explicitly re-summons your last companion on demand.

- **Improved Randomization Logic:**  
  Refined how the pet pool is built and picked from, reducing streaks and “stuck on one pet” behavior.

### 🧩 UI & UX Updates
- **Pet Manager:**
  - Favorite checkbox alignment fixed under the **Favorite** column header.
  - Layout adapts better to window width and UI scale.
  - Scroll area and row anchoring fixed so checkboxes and counts always show correctly.

- **Options Panel:**
  - Zone-related controls removed (to match current feature set).
  - Random Mode dropdown text correctly reflects the selected mode instead of showing “Custom”.
  - Overall improved spacing and scrollbar behavior.

- **Summon & Minimap Buttons:**
  - Tooltips now show the currently summoned pet (icon + name).
  - Left-click: summon; Right-click: open Options.
  - Minimap button remains positioned just outside the minimap ring and is draggable.

### 🧰 Technical
- Cleaned up dead code for holidays and zone sets (Retail build).
- Added `APKDB.recent` SavedVariable to track recent summons for anti-repeat.
- Ensured safe initialization when upgrading from older versions.

---

## v1.2.0 — Retail
- Added **Pet Manager** for viewing:
  - Favorites
  - Blacklisted pets
  - Summon counts
- Added **Options panel** with:
  - Auto-summon toggles
  - Location filters (indoors/outdoors/raid)
  - Random Mode selection (Any/Flying/Non-Flying)
  - Minimap button toggle
- Added **Minimap Button** (summon/options + draggable).
- Introduced initial **zone-based pet sets** (now removed in v1.3.0 for stability).

---

## v1.0.0 — Initial Retail Release
- Basic random summoning from your pet collection.
- Favorites + blacklist system.
- Simple `/apk` and `/apk options` commands.
