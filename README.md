# Graph Implementation

This project implements an undirected and unweighted graph in C++ with functionality to:
- Add vertices
- Add edges
- Find the shortest path between two vertices using BFS
- Print the path

## Files

### 1. `Graph.cpp`
Contains the implementation of graph operations:
- **`addEdge(int v1, int v2)`**: Adds an undirected edge between vertices `v1` and `v2`.
- **`addVertex(int n)`**: Adds a vertex with key `n` to the graph if it doesn't already exist.
- **`printPath(int src, int dest)`**: Prints the vertices in the shortest path between `src` and `dest`.
- **`findShortestPath(int src, int dest)`**: Finds the shortest path length between `src` and `dest` using Breadth-First Search (BFS).

### 2. `Graph.hpp`
Header file defines the structures and class methods:
- **Structures**:
  - `vertex`: Represents a graph vertex, with properties like `key`, `visited`, `distance`, and adjacency list.
  - `adjVertex`: Represents an adjacent vertex in the adjacency list.
- **Class**:
  - `Graph`: Encapsulates graph functionality, including methods for adding vertices, adding edges, and finding paths.

### 3. `main.cpp`
Driver program demonstrates the graph operations:
- Creates a graph with 6 vertices and edges.
- Uses `findShortestPath` to calculate the shortest path length between vertex 1 and 6.
- Calls `printPath` to display the shortest path (currently incomplete).

## How to Compile and Run
Use the following commands to compile and execute:

```bash
g++ -o graph main.cpp Graph.cpp
./graph
