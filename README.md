# ❄️ Cleaners vs Snow

An engaging, text-based terminal strategy and clicker game written in Python. Players face an economic and environmental dilemma: take control of a commercial **Snow Cleaning Company** to systematically clear winter hazards, or control the **Snow Weather** itself to blanket the grid and disrupt operations.

## ✨ Core Features
* **Dual-Faction Gameplay**: Play two completely distinct simulation loops with unique progression tracks.
* **Incremental Economy**: Use active terminal interaction (`Enter` farming) combined with automated tool upgrades and scaling multipliers.
* **Persistent States**: State-serialization system utilizing native JSON structures (`save.json`, `snow.json`, `company.json`) to safely load or write progress.
* **Modular Codebase**: Clean, decoupled architectural design separating core runtime execution (`main.py`) from entities (`player.py`), rendering (`printer.py`), and storage routines (`saves.py`).

## 📁 Repository Structure
* `main.py` — Primary application entryway initializing main menus and scheduling the global game loops.
* `player.py` — Base object class structures managing inventory indexes, currency counters, and tool tier calculations.
* `printer.py` — High-utility terminal rendering layout module providing formatting structures for text-art screens.
* `saves.py` — Input/Output buffer pipeline managing file locks and deep state JSON formatting.

## 🚀 Installation & Setup

### Prerequisites
Make sure you have **Python 3.8+** installed on your operating system.

### Deployment Steps
1. Clone the project tree:
   ```bash
   git clone https://github.com
   ```
2. Step inside the application root environment:
   ```bash
   cd snow-game
   ```
3. Install required setup dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## 🎮 How to Play
1. **Launch the Engine**: Start the terminal execution loop:
   ```bash
   python3 main.py
   ```
2. **Faction Select**: Pick your alliance (Snow Cleaning Enterprise OR Overlord Weather System).
3. **Resource Farming**: Press `Enter` to generate operational capital (Coins or Precipitation Density).
4. **Acquire Upgrades**: Open the in-game market window to buy automated machinery, deploy workforce boosts, or optimize passive production efficiency.

---
❄️ *Will you clean the town or bury it under the drift? The forecast is up to you.*
