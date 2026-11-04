# coin-change-state-space-explorer-project
 Coin Change State Space Explorer — BFS &amp; A* Algorithm Visualization
# 🪙 Coin Change State Space Explorer — BFS & A* Algorithm Visualization

An interactive, educational, and visually rich web application built to demonstrate state-space graph search algorithms (**Breadth-First Search** and **A* Search**) applied to the classic **Coin Change Problem**. 

This application visualizes how tree/graph search algorithms systematically explore state spaces to determine the optimal minimum coin sequence for any given target amount.

---

## 🌟 Key Features

* **State Space Graph & Tree Visualization:** Visualizes nodes as accumulated amounts and edges as coin additions (`+coin`), highlighting active, visited, and goal states in real-time using SVG vectors.
* **Dual Search Engines:**
  * **BFS (Breadth-First Search):** Guarantees optimal coin count by exploring states level-by-level using a FIFO Queue.
  * **A* Search Algorithm:** Guided search using a Min-Priority Queue powered by an admissible heuristic:
    $$h(n) = \left\lceil \frac{\text{Target} - \text{Current Amount}}{\text{Max Coin}} \right\rceil$$
* **Interactive Step Playback:** Full animation controls including **Play**, **Pause**, **Step Forward**, **Step Back**, **Replay**, and variable execution speed settings ($0.5x$, $1x$, $2x$, $4x$).
* **Real-time Metrics & Statistics:** Displays generated states, expanded states, max frontier size, execution duration in milliseconds, and live step event logs.
* **Side-by-Side Comparison:** Compares BFS and A* algorithm efficiency and performance directly.
* **Preset Configuration Library:** Features quick-load educational test cases (*Simple Example*, *Greedy Trap*, *Larger Target*, *Unreachable*, and *Zero Target*).
* **Strict Numeric Formatting:** Displays amounts as clean numbers only without any currency symbols or codes.

---

## 🛠️ Technology Stack

* **HTML5 & Modern CSS3**
* **React 18** (Standalone UMD)
* **Tailwind CSS** (Utility-first styling with dark theme palette)
* **Babel Standalone** (Client-side JSX transformation)
* **SVG (Scalable Vector Graphics)** for graph network dynamic layout

---

## 🚀 How to Run Locally

Because this project is built as a self-contained web app, running it is simple and does not require complex setup or package installations:

1. Clone or download this repository:
   ```bash
   git clone https://github.com/YOUR_USERNAME/coin-change-state-space-explorer.git
   ```
2. Navigate into the directory:
   ```bash
   cd coin-change-state-space-explorer
   ```
3. Open `index.html` directly in any modern web browser (Google Chrome, Mozilla Firefox, Edge, Safari).

---

## 📸 State Space Graph Legend

| Node State | Color | Description |
| :--- | :--- | :--- |
| **Active State** | 🔵 Blue Glow | Currently expanded state being processed |
| **Goal State** | 🟢 Emerald Green | Target amount reached successfully |
| **Visited State** | 🩶 Dark Charcoal | Explored state stored in memory |
| **Edge Transitions** | ↗️ Dashed Line | Represents adding a specific coin denomination (`+coin`) |

---

## 📜 License

This project is licensed under the **MIT License** — feel free to use, modify, and distribute for educational and academic purposes.
