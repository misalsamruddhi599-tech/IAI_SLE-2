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
- Number of Runs: 3
- Algorithms: BFS and DFS

### Graph Structure :

Each node is connected to the next four available nodes.

```text
0  →  1, 2, 3, 4
1  →  2, 3, 4, 5
2  →  3, 4, 5, 6
3  →  4, 5, 6, 7
4  →  5, 6, 7, 8
...
1195 → 1196, 1197, 1198, 1199
1196 → 1197, 1198, 1199
1197 → 1198, 1199
1198 → 1199
1199 → No next node

The graph was generated programmatically using the same connection rule for all 1200 nodes.

Test Cases :
Best Case: Goal Node = 1
Average Case: Goal Node = 600
Worst Case: Goal Node = 1199

 ## 4. Profiling Method :

The performance of both algorithms was measured using Python's timeit module.

The following metrics were measured:

Execution time in milliseconds.
Number of nodes expanded.
Goal-search success.

Each algorithm was executed three times for each test case on the same graph. The average execution time was calculated from the three runs.

The number of expanded nodes was counted manually during the search.

> ### 5. Experimental Results :

Best Case – Goal Node 1
Metric	BFS	DFS
Run 1 Time (ms)	0.16890	0.10150
Run 2 Time (ms)	0.09670	0.09630
Run 3 Time (ms)	0.09450	0.12500
Average Time (ms)	0.12003	0.10760
Nodes Expanded	2	2
Goal Found	True	True
Average Case – Goal Node 600
Metric	BFS	DFS
Run 1 Time (ms)	36.70380	12.00910
Run 2 Time (ms)	29.63510	13.26550
Run 3 Time (ms)	35.04990	11.47430
Average Time (ms)	33.79627	12.24963
Nodes Expanded	601	241
Goal Found	True	True
Worst Case – Goal Node 1199
Metric	BFS	DFS
Run 1 Time (ms)	60.58080	25.93440
Run 2 Time (ms)	63.67570	24.21780
Run 3 Time (ms)	60.71790	23.81700
Average Time (ms)	61.65813	24.65640
Nodes Expanded	1200	483
Goal Found	True	True
6. Observation :

DFS required less average execution time than BFS in all three selected test cases.

In the Best Case, both algorithms expanded 2 nodes.

In the Average Case and Worst Case, DFS expanded fewer nodes than BFS and also showed lower average execution time.

7. Justification and Analysis :

Based on the measured results, DFS showed lower average execution time than BFS for the given graph and experimental setup.

In the Best Case, BFS took 0.12003 ms and DFS took 0.10760 ms, with both expanding 2 nodes.

In the Average Case, BFS took 33.79627 ms and expanded 601 nodes, while DFS took 12.24963 ms and expanded 241 nodes.

In the Worst Case, BFS took 61.65813 ms and expanded 1200 nodes, while DFS took 24.65640 ms and expanded 483 nodes.

Both algorithms successfully found the goal node in all test cases.

The comparison is based on actual measurements obtained using the timeit method.

Performance may change for a different graph structure, traversal order, or problem size.

8. Conclusion :

This profiling experiment helped in understanding the practical performance of BFS and DFS.

Execution time and nodes expanded were measured using the same graph for both algorithms.

DFS showed lower average execution time in all three selected test cases.

DFS also expanded fewer nodes than BFS in the Average Case and Worst Case.

The experiment demonstrated the importance of empirical profiling along with theoretical analysis.

9. AI Contribution :

ChatGPT was used as an assistance tool during the development and documentation of this SLE-2.

AI assistance included:

Preparing the BFS and DFS profiling code.
Setting up execution-time measurement using timeit.
Adding node-counting functionality.
Setting up the graph creation logic.
Organizing Best Case, Average Case and Worst Case testing.
Organizing the experimental results.
Assisting with the structure and wording of the SLE-2 documentation.

The program was executed by the student, and the actual experimental results were collected from the program execution.

10. Project Files :
bfs_vs_dfs.py – Python implementation of BFS and DFS with profiling.
README.md – Project description, graph structure, profiling method, and experimental results.
AI_Contribution_Log.md – Detailed record of AI assistance and student contribution.
SLE-2_Profiling_Report.pdf – Final SLE-2 profiling report.
11. Final Result :

BFS Best Case Average Time: 0.12003 ms

DFS Best Case Average Time: 0.10760 ms

BFS Average Case Average Time: 33.79627 ms

DFS Average Case Average Time: 12.24963 ms

BFS Worst Case Average Time: 61.65813 ms

DFS Worst Case Average Time: 24.65640 ms

BFS Best Case Nodes Expanded: 2

DFS Best Case Nodes Expanded: 2

BFS Average Case Nodes Expanded: 601

DFS Average Case Nodes Expanded: 241

BFS Worst Case Nodes Expanded: 1200

DFS Worst Case Nodes Expanded: 483

BFS Goal Found: True

DFS Goal Found: True

For this particular graph and experimental setup, DFS showed lower average execution time in all three selected test cases and expanded fewer nodes in the Average Case and Worst Case.