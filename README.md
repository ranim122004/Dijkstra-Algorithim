# Dijkstra Shortest-Path — Maze Visualizer

An interactive **Dijkstra’s algorithm** maze app: build a maze, place hurdles (costly cells/agents), run Dijkstra to reveal the **shortest path**, visualize the traversal, and reset to try new layouts.

## ✨ Features

- **Maze generation** with configurable rows/columns and optional loops.  
- **Costed hurdles** (red agents) that influence path cost.  
- **Run Dijkstra** to compute shortest path and total cost; results **rendered on the maze**.  
- **Animated tracing** of the computed path; **Reset** to experiment again.

> Internally, the run loop repeatedly picks the unvisited node with **minimum tentative distance**, relaxes neighbors, and reconstructs the path from predecessor links—classic Dijkstra. :contentReference[oaicite:1]{index=1}

---

## 🧠 Why Dijkstra?

Dijkstra’s algorithm solves the **single-source shortest path** problem on graphs with **non-negative** edge weights, producing a shortest-path tree. It commonly uses a **min-priority queue** to select the next node, giving a time complexity of  
- **O((|V| + |E|) log |V|)** with a binary heap, or  
- **O(|E| + |V| log |V|)** with a Fibonacci heap. :contentReference[oaicite:2]{index=2}


## 🛠 Tech Stack

- **Python 3.x**  
- **Maze/agents & path tracing:** `pyamaze` (for `CreateMaze`, `agent`, `tracePath`, `textLabel`) :contentReference[oaicite:4]{index=4}

---

## 🚀 Getting Started

1) **Clone**
```bash
git clone https://github.com/<your-username>/<your-repo>.git
cd <your-repo>
