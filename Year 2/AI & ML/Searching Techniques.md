___

# Uninformed search/ Blind search strategy:

- **Does not use** any domain-specific knowledge.
- **Explores all possible paths** without guidance.
- **Only uses problem definition** (initial state, actions, goal test).    
- **Matches all states with goal state** blindly.
 
- Examples:
    - Breadth-First Search (BFS)
    - Depth-First Search (DFS)
    - Uniform Cost Search (UCS)
    - Depth-Limited Search
    - Iterative Deepening Search

# Informed search

- Uses **heuristics or additional domain knowledge** to guide the search.
- **Estimates cost** or distance to the goal using a heuristic function h(n).
- **More efficient** than uninformed search—explores fewer nodes.
- Prioritizes **promising paths** based on heuristic evaluation.
- Does **not guarantee optimality** unless using an admissible heuristic (e.g., in A* search).
- Examples:
    - **Greedy Best-First Search** – chooses the node with the lowest h(n)
    - _A Search_* – chooses based on f(n) = g(n) + h(n) (cost so far + estimated cost)
    - **Recursive Best-First Search (RBFS)**
    - **Memory Bounded A*** (e.g., IDA*, SMA*)


### Initial State (State 1)
Heuristic h(n) = 3 (Misplaced tiles: 4, 5, 8)

| 1 | 2 | 3 |
|---|---|---|
|   | 4 | 6 |
| 7 | 5 | 8 |

---

### State A – Move 4 Left (swap blank and 4)
Heuristic h(n) = 3 (Misplaced tiles: 4, 5, 8)

| 1 | 2 | 3 |
|---|---|---|
| 4 |   | 6 |
| 7 | 5 | 8 |

---

### State B – Move 6 Left (swap blank and 6)
Heuristic h(n) = 4 (Misplaced tiles: 4, 5, 6, 8)

| 1 | 2 | 3 |
|---|---|---|
| 4 | 6 |   |
| 7 | 5 | 8 |

---

### State C – Move 7 Up (swap blank and 7)
Heuristic h(n) = 5 (Misplaced tiles: 4, 5, 6, 7, 8)

| 1 | 2 | 3 |
|---|---|---|
| 7 | 4 | 6 |
|   | 5 | 8 |

### Greedy (informed approach)

