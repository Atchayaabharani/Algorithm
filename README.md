# A* Algorithm

# A* Search Algorithm in Python (Generic Graph Version)

This project contains a **Python implementation of the A\* (A-star) Search Algorithm** that works on **any weighted graph**.  
It can also work as **Dijkstra’s Algorithm** by simply using a zero-valued heuristic.

---

## 📌 Features
- Works with **any weighted graph** (not just grids or coordinates).
- Easy to switch between **A\*** and **Dijkstra**:
  - A\* → Use a custom heuristic.
  - Dijkstra → Use a zero heuristic.
- Returns the **shortest path** between two nodes.
- Uses **Python’s `heapq`** for priority queue efficiency.

---

## 📂 How the Code Works
1. **Graph Representation**  
   The graph is stored as a **dictionary**:
   ```python
   graph = {
       'A': [('B', 1), ('C', 3)],
       'B': [('A', 1), ('C', 1), ('D', 3)],
       'C': [('A', 3), ('B', 1), ('D', 1), ('E', 5)],
       'D': [('B', 3), ('C', 1), ('E', 2)],
       'E': [('C', 5), ('D', 2)]
   }
