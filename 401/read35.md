# Read: Class 35 : Graphs

---

**_A graph_** is a non-linear data structure that can be looked at as a collection of vertices (or nodes) potentially connected by line segments named edges.

- **_Vertex_** - A vertex, also called a “node”, is a data object that can have zero or more adjacent vertices.
- **_Edge_** - An edge is a connection between two nodes.
- **_Neighbor_** - The neighbors of a node are its adjacent nodes, i.e., are connected via an edge.
- **_Degree_** - The degree of a vertex is the number of edges connected to that vertex.

### Undirected Graphs

**_Undirected Graph_** is a graph where each edge is undirected or bi-directional. This means that the undirected graph does not move in any direction

Vertices/Nodes = {a,b,c,d,e,f}

Edges = {(a,c),(a,d),(b,c),(b,f),(c,e),(d,e),(e,f)}

![](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/assets/UndirectedGraph.PNG)

### Directed Graphs (Digraph)

A **_Directed Graph _** also called a **_Digraph_** is a graph where every edge is directed.

Unlike an undirected graph, a Digraph has direction. Each node is directed at another node with a specific requirement of what node should be referenced next.

![](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/assets/DirectedGraph.PNG)

Vertices = {a,b,c,d,e,f}

Edges = {(a,c),(b,c),(b,f),(c,e),(d,a),(d,e)(e,c)(e,f)}

## Complete vs Connected vs Disconnected

This depends on how connected the graphs are to other node/vertices.

- **_Complete Graphs _** A complete graph is when all nodes are connected to all other nodes.

- A **_connected graph_** is graph that has all of vertices/nodes have at least one edge.

- A **_disconnected graph_** is a graph where some vertices may not have edges.

## Acyclic vs Cyclic

- **_Acyclic Graph_** An acyclic graph is a directed graph without cycles.

A cycle is when a node can be traversed through and potentially end up back at it

- A **_Cyclic graph_** is a graph that has cycles.

A cycle is defined as a path of a positive length that starts and ends at the same vertex.

## Graph Representation

We represent graphs through:


- **_Adjacency Matrix_** An Adjacency matrix is represented through a 2-dimensional array. If there are n vertices, then we are looking at an n x n Boolean matrix

- **_Adjacency List_** An adjacency list is the most common way to represent graphs.An adjacency list is a collection of linked lists or array that lists all of the other vertices that are connected.Adjacency lists make it easy to view if one vertices connects to another.

### Real World Uses of Graphs

Graphs are extremely popular when it comes to it’s uses. Here are just a few examples of graphs in use:

- GPS and Mapping
- Driving Directions
- Social Networks
- Airline Traffic
- Netflix uses graphs for suggestions of products
