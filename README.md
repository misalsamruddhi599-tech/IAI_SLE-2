# SLE-2: Empirical Performance Analysis


## 1. AIM :

To experimentally compare the performance of Breadth First Search (BFS) and Depth First Search (DFS) using actual execution time and the number of nodes expanded.

---

## 2. Algorithms Used :

### BFS – Breadth First Search

BFS is an uninformed search algorithm that explores nodes level by level. It uses a queue to manage the nodes waiting to be explored.

### DFS – Depth First Search

DFS is an uninformed search algorithm that explores one path as deeply as possible before backtracking. It uses a stack to manage the nodes during the search.

---

## 3. Problem Configuration :

The same graph was used for both BFS and DFS.

- Number of Nodes: 1200
- Start Node: 0
- Goal Node: 1199
- Number of Runs: 3
- Algorithms: BFS and DFS

---

## 4. Profiling Method :

The performance of both algorithms was measured using Python's `timeit` module.

The following metrics were measured:

1. Execution time in milliseconds.
2. Number of nodes expanded.
3. Goal-search success.

Each algorithm was executed three times on the same graph. The average execution time was calculated from the three runs.

The number of expanded nodes was counted manually during the search.

---

## 5. Experimental Results :

| Metric | BFS | DFS |
|---|---:|---:|
| Run 1 Time (ms) | 191.72740 | 133.69550 |
| Run 2 Time (ms) | 154.22590 | 142.94200 |
| Run 3 Time (ms) | 166.97830 | 132.48120 |
| Average Time (ms) | 170.97720 | 136.37290 |
| Average Nodes Expanded | 1200 | 1200 |
| Goal Found | True | True |

---

## 6. Observation :

DFS required less average execution time than BFS in this experiment.

Both algorithms expanded the same number of nodes (1200), while DFS showed the lower average execution time.

---

## 7. Justification and Analysis :

Based on the measured results, DFS performed faster than BFS for the given graph.

The average execution time of DFS was 136.37290 ms, while BFS took 170.97720 ms.

Both algorithms expanded 1200 nodes during the search.

Therefore, the main performance difference in this experiment was execution time rather than the number of nodes expanded.

Both algorithms successfully found the goal node 1199.

The comparison is based on actual measurements obtained using the `timeit` method.

Performance may change for a different graph structure or problem size.

---

## 8. Conclusion :

This profiling experiment helped in understanding the practical performance of BFS and DFS.

Execution time and nodes expanded were measured using the same graph for both algorithms.

DFS showed lower average execution time, while both algorithms expanded the same number of nodes in this experiment.

The experiment helped demonstrate the importance of empirical profiling along with theoretical analysis.

---

## 9. AI Contribution :

ChatGPT was used as an assistance tool during the development and documentation of this SLE.

AI assistance included:

- Preparing the BFS and DFS profiling code.
- Setting up execution-time measurement using `timeit`.
- Adding node-counting functionality.
- Organizing the experimental results.
- Assisting with the structure and wording of the SLE-2 report.

The program was executed by the student, and the actual experimental results were collected from the program execution.

---

## 10. Project Files :

- `bfs_vs_dfs.py` – Python implementation of BFS and DFS with profiling.
- `README.md` – Project description, profiling method, and experimental results.
- `AI_Contribution_Log.md` – Detailed record of AI assistance.
- `SLE-2_Profiling_Report.pdf` – Final SLE-2 profiling report.

---

## 11. Final Result :

**BFS Average Time:** 170.97720 ms  
**DFS Average Time:** 136.37290 ms  

**BFS Average Nodes Expanded:** 1200  
**DFS Average Nodes Expanded:** 1200  

**BFS Goal Found:** True  
**DFS Goal Found:** True  

> For this particular graph and experimental setup, DFS showed lower average execution time than BFS.