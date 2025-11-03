Smart City Scheduling - Graph Algorithms
A Java implementation of graph algorithms for urban task scheduling, featuring Strongly Connected Components (SCC), Topological Sorting, and DAG Shortest Path calculations.

 -Project Overview
This project implements three core graph algorithms:

Strongly Connected Components (SCC) using Tarjan's algorithm

Topological Sorting using Kahn's algorithm

Shortest/Longest Paths in Directed Acyclic Graphs (DAGs)

Algorithms Implemented
1. Strongly Connected Components (Tarjan's Algorithm)
   Time Complexity: O(V + E)

Space Complexity: O(V)

Output: List of SCCs and their sizes

2. Topological Sort (Kahn's Algorithm)
   Time Complexity: O(V + E)

Space Complexity: O(V)

Output: Valid topological order of the condensation DAG
3. DAG Shortest Paths
   Time Complexity: O(V + E)

Output:

Smart City Scheduling Analysis 
Nodes: 8
Edges: 7
Source: 4
Weight Model: edge

 Strongly Connected Components 
Number of SCCs: 5
SCC 0: [0] (size: 1)
SCC 1: [1, 2, 3] (size: 3)
SCC 2: [4] (size: 1)
SCC 3: [5] (size: 1)
SCC 4: [6, 7] (size: 2)

Condensation Graph & Topological Sort 
Topological Order: [4, 0, 1, 5, 2, 3, 6]

 Shortest and Longest Paths 
Shortest Paths from source 4:
to 4: 0 (path: [4])
to 5: 2 (path: [4, 5])
to 6: 7 (path: [4, 5, 6])
to 7: 8 (path: [4, 5, 6, 7])
Critical Path (Longest):
Length: 8
Path: [4, 5, 6, 7]
 Performance Metrics
 The implementation includes instrumentation for:

Operation counts (DFS visits, queue operations, relaxations)

Execution time in nanoseconds

Memory usage patterns

Use Cases
Urban Task Scheduling: Street cleaning, repairs, maintenance

Project Management: Critical path analysis

Dependency Resolution: Task ordering with constraints

Network Analysis: Connectivity and routing

Configuration
Weight Model
The project uses edge weights as specified in the assignment. Node durations can be implemented by modifying the weight model.

Graph Types Supported
Cyclic graphs: Automatically detected and compressed via SCC

DAGs: Direct topological sorting and path calculation

Mixed graphs: SCC compression followed by DAG algorithms
