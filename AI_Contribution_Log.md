## AI Contribution Log :

## SLE-2: Empirical Performance Analysis :

## 1. AI Tool Used :

AI Tool: ChatGPT

ChatGPT was used as a supporting tool during the development, profiling, and documentation of the SLE-2 experiment.

# 2. Purpose of AI Assistance :

AI assistance was used to support the preparation of the BFS and DFS profiling implementation and to organize the experimental results, graph description, and documentation.

## 3. Contribution of AI :

Code Preparation

ChatGPT assisted with preparing the Python code for:

-Breadth First Search (BFS)
-Depth First Search (DFS)
-Graph creation
-Node counting
-Execution-time measurement
-Multiple experimental runs
-Average execution-time calculation
-Best Case, Average Case and Worst Case testing
-Graph Setup

ChatGPT assisted in defining and documenting the graph used in the experiment.

Number of nodes: 1200
Start node: 0
Each node is connected to the next 4 available nodes.

Representative structure:

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
Profiling Setup

ChatGPT assisted in setting up Python's timeit module for measuring the execution time of BFS and DFS.

Manual node counting was also included to measure the number of nodes expanded by each algorithm.

Result Organization

ChatGPT helped organize the output into a comparison containing:

-Run 1 execution time
-Run 2 execution time
-Run 3 execution time
-Average execution time
-Nodes expanded
-Goal-found status
-Report Preparation

ChatGPT assisted in organizing the SLE-2 documentation into the required sections and preparing the README and AI Contribution Log.

4. Student's Own Contribution :

-The student:

-Understood the BFS and DFS algorithms.

-Reviewed and used the profiling code.

-Executed the program in VS Code.

-Ran both algorithms for three runs in each test case.

-Collected the actual execution results.

-Checked the goal-found status.

-Compared the measured execution times.

-Compared the number of nodes expanded.

-Used the actual results for the final analysis.

-Prepared the final submission files.

## 5. Actual Experimental Results :

Best Case – Goal Node 1 :

Metric	BFS	DFS
Run 1 Time (ms)	0.16890	0.10150
Run 2 Time (ms)	0.09670	0.09630
Run 3 Time (ms)	0.09450	0.12500
Average Time (ms)	0.12003	0.10760
Nodes Expanded	2	2
Goal Found	True	True

Average Case – Goal Node 600 :

Metric	BFS	DFS
Run 1 Time (ms)	36.70380	12.00910
Run 2 Time (ms)	29.63510	13.26550
Run 3 Time (ms)	35.04990	11.47430
Average Time (ms)	33.79627	12.24963
Nodes Expanded	601	241
Goal Found	True	True

Worst Case – Goal Node 1199 :

Metric	BFS	DFS
Run 1 Time (ms)	60.58080	25.93440
Run 2 Time (ms)	63.67570	24.21780
Run 3 Time (ms)	60.71790	23.81700
Average Time (ms)	61.65813	24.65640
Nodes Expanded	1200	483
Goal Found	True	True

## 6. Result Interpretation :

For the given graph and experimental setup, DFS had a lower average execution time in all three selected test cases.

In the Best Case, both algorithms expanded 2 nodes.

In the Average Case, BFS expanded 601 nodes, while DFS expanded 241 nodes.

In the Worst Case, BFS expanded 1200 nodes, while DFS expanded 483 nodes.

Therefore, based on the actual measured results, DFS showed lower execution time and fewer expanded nodes in the Average and Worst Case tests.

## 7. AI Usage Statement :

AI was used as an assistance tool for code preparation, graph setup, profiling configuration, explanation, result organization, and documentation.

The actual program execution and collection of performance results were performed by the student.

The final comparison and analysis were based on the actual measured experimental results.

## 8. Declaration :

> I have used AI assistance transparently for the tasks mentioned above and have verified the experimental results obtained from my program.