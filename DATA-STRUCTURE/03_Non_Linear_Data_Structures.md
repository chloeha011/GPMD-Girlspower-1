# Non-Linear Data Structures

## 1. Definition

A non-linear data structure organizes data in a hierarchical or network-like form rather than in one single sequence. A node can connect to more than one other node, allowing the structure to represent branching relationships and multiple possible paths.

The two main examples are **trees** and **graphs**. Trees represent hierarchical relationships, such as folders within a computer. Graphs represent general connections, such as roads between locations or friendships in a social network.

Unlike linear structures such as arrays and queues, non-linear structures are useful when data has branching relationships or complex connections.

### Linear vs. Non-Linear Data Structures

- **Linear:** Elements follow one logical sequence. Examples include arrays, linked lists, stacks, and queues.
- **Non-linear:** Elements can have branching or network-like connections. Examples include trees and graphs.

## 2. How Non-Linear Data Structures Work

Non-linear data structures are commonly described using **nodes** and **connections**.

- **Node:** An individual unit that stores data.
- **Edge:** A connection between two nodes. In a tree, edges usually represent parent-child relationships.

A program starts from a chosen node, such as the root of a tree or a starting vertex in a graph, and follows connections using a traversal or search algorithm.

### General Process

1. Create nodes to store the data.
2. Connect nodes according to the relationships being represented.
3. Choose a starting node when an operation requires one.
4. Traverse or search the structure using a suitable algorithm.
5. Add, remove, or update nodes and connections when the data changes.

### Memory Organization

Non-linear structures can be stored in different ways:

- **Linked representation:** Nodes store references to other nodes. This is common in trees and adjacency-list graphs.
- **Array-based representation:** Values are stored in arrays and related through index positions. Binary heaps are commonly implemented this way.
- **Adjacency matrix:** A two-dimensional array records whether pairs of graph vertices are connected. It can also store edge weights.

The choice of representation affects memory use and the speed of operations.

## 3. Characteristics of Non-Linear Data Structures

- **Multiple connections:** A node may connect to several other nodes.
- **Branching or network organization:** Data can form levels or interconnected networks.
- **Different traversal orders:** Algorithms can visit nodes in different sequences.
- **Relationship-based organization:** Useful for representing dependencies and connections.
- **Flexible structure:** Many implementations allow nodes and connections to be added or removed.
- **Implementation-dependent performance:** Search and update times depend on the structure, its representation, and the algorithm used.

## 4. Main Types of Non-Linear Data Structures

The two main types are trees and graphs. Heaps and tries are specialized tree-based structures.

### 4.1 Trees

A **tree** is a hierarchical structure made of nodes connected by edges. A rooted tree has one starting node called the **root**. Other nodes are arranged below it in parent-child relationships.

A conventional tree with \(n\) nodes has exactly \(n-1\) edges. It is connected and contains no cycles.

### Example of a Tree

```
        A
       / \
      B   C
     / \ / \
    D  E F  G
```

A is the root. B and C are children of A. D, E, F, and G are leaf nodes.

### Important Terminology

- **Root:** The topmost node of a rooted tree.
- **Parent:** A node directly above one or more child nodes.
- **Child:** A node directly below a parent.
- **Leaf:** A node with no children.
- **Edge:** A connection between two nodes.
- **Subtree:** A node together with all its descendants.
- **Depth:** The number of edges from the root to a particular node.
- **Height:** The number of edges on the longest downward path from a node to a leaf. The height of a tree is the height of its root.

### How a Tree Works

1. Data is stored in nodes.
2. A root node provides the starting point.
3. Other nodes are connected through parent-child relationships.
4. A traversal algorithm visits nodes in a defined order.
5. Search and insertion operations follow the rules of the particular tree type.

### Common Types of Trees

- **Binary tree:** Each node has at most two children.
- **Binary search tree (BST):** For the standard distinct-key version, values in the left subtree are smaller than the node's value, and values in the right subtree are larger.
- **Heap:** A complete binary tree that follows a heap-order rule. In a max-heap, each parent is greater than or equal to its children; in a min-heap, each parent is less than or equal to its children.
- **Trie:** A tree-like structure that stores sequences, commonly words, by shared prefixes.

### Advantages

- Represents hierarchical information naturally.
- Can support efficient searching and insertion when appropriately structured.
- Organizes information into clear levels.

### Limitations

- More complex to implement than basic linear structures.
- An unbalanced binary search tree can become less efficient, with some operations taking O(n) time.
- Traversal and memory management require additional logic.

### Applications

- Computer file systems.
- Organizational charts.
- Database indexing.
- Search operations.
- Autocomplete and word prediction.

### 4.2 Graphs

A **graph** is a non-linear data structure consisting of **vertices** (also called nodes) and **edges** that connect pairs of vertices. Unlike a tree, a general graph can contain cycles, and a vertex can connect to many others without following a parent-child hierarchy.

A graph is commonly represented as:

\[
G = (V, E)
\]

where:

- \(V\) is the set of vertices.
- \(E\) is the set of edges connecting vertices.

### Example of a Graph

```
A ----- B
|       |
|       |
C ----- D
```

Each letter represents a vertex, and each line represents an edge. The connections create more than one possible path between some vertices.

### Important Terminology

- **Vertex:** An individual node in a graph.
- **Edge:** A connection between two vertices.
- **Adjacent vertices:** Two vertices connected directly by an edge.
- **Degree:** The number of edges connected to a vertex in an undirected graph.
- **Path:** A sequence of vertices connected by edges.
- **Cycle:** A path that starts and ends at the same vertex.
- **Weight:** A value assigned to an edge, such as distance, cost, or time.

### How a Graph Works

1. Define vertices to represent objects or entities.
2. Create edges to represent relationships between them.
3. Store the connections using an adjacency list or adjacency matrix.
4. Use algorithms to explore the graph, find paths, or identify relationships.
5. Update vertices, edges, or weights when the network changes.

### Common Types of Graphs

- **Undirected graph:** Edges have no direction; a connection works both ways.
- **Directed graph:** Edges have a direction, such as \(A \rightarrow B\).
- **Weighted graph:** Edges have values such as cost, distance, or time.
- **Unweighted graph:** Edges represent connections without assigned weights.
- **Cyclic graph:** Contains at least one cycle.
- **Acyclic graph:** Contains no cycles. A directed acyclic graph (DAG) is often used to represent tasks or dependencies.

### Advantages

- Represents complex relationships naturally.
- Supports pathfinding and network analysis.
- Models real-world systems with many interconnected entities.

### Limitations

- An adjacency matrix can use substantial memory for a large, sparse graph.
- Searching and traversal may become expensive for large networks.
- Some graph problems require advanced algorithms.

### Applications

- Social networks.
- Road and transportation networks.
- Computer networks.
- Recommendation systems.
- Project scheduling and dependency management.
- Knowledge representation in artificial intelligence.

## 5. Comparison of Trees and Graphs

| Feature | Tree | General Graph |
| --- | --- | --- |
| Organization | Hierarchical | Network-like |
| Connections | Parent-child relationships | General vertex-to-vertex relationships |
| Root | A rooted tree has one root | No root is required |
| Cycles | No cycles | May contain cycles |
| Connectivity | Connected by definition | May be connected or disconnected |
| Number of edges | A tree with \(n\) nodes has \(n-1\) edges | Depends on the graph |
| Typical applications | File systems, search trees | Social networks, routes, dependencies |

A tree is a special type of graph: it is connected and has no cycles. However, not every graph is a tree.

## 6. Traversal of Non-Linear Data Structures

**Traversal** is the process of visiting nodes in a data structure to inspect or process their data. Since non-linear structures can branch or contain multiple paths, algorithms are used to determine the order in which nodes are visited.

### 6.1 Breadth-First Search (BFS)

BFS explores nodes level by level, visiting nearby nodes before moving farther away. It typically uses a **queue** to keep track of which node to visit next.

### 6.2 Depth-First Search (DFS)

DFS explores one path as far as possible before returning to explore another path. It typically uses a **stack** or recursion.

### Common Tree Traversal Methods

For a binary tree, common traversal methods include:

- **Preorder:** Visit the root, then the left subtree, then the right subtree.
- **Inorder:** Visit the left subtree, then the root, then the right subtree.
- **Postorder:** Visit the left subtree, then the right subtree, then the root.
- **Level-order:** Visit nodes level by level, typically using a queue.

The choice of traversal depends on the task. For example, BFS can find a shortest path in an unweighted graph, while DFS is useful for exploring connected regions and checking relationships.

### Traversal Complexity

For a graph represented with an adjacency list, BFS and DFS take \(O(V + E)\) time, where \(V\) is the number of vertices and \(E\) is the number of edges. This is because the algorithms visit vertices and examine edges. With an adjacency matrix, traversal commonly takes \(O(V^2)\) time.

## 7. Worked Example: Finding a Shortest Path Using BFS

Suppose a small transport network has four locations connected as follows:

- A connects to B and C.
- B connects to D.
- C connects to D.

The network can be represented as:

```
    A
   / \
  B   C
   \ /
    D
```

**Task:** Find a shortest path from A to D using BFS, exploring B before C.

1. **Start at A.** Add its unvisited neighbors B and C to the queue.

   Queue: `[B, C]`

2. **Visit B.** Discover D and add it to the queue.

   Queue: `[C, D]`

3. **Visit C.** D has already been discovered, so do not add it again.

   Queue: `[D]`

4. **Visit D.** The target has been reached.

**Expected result:** One shortest path is `A → B → D`, which contains two edges. The alternative path `A → C → D` also contains two edges.

This example shows how BFS explores a graph level by level. In an unweighted graph, BFS finds a path with the fewest edges.

## 8. Learner Activity

Consider the following tree:

```
        10
       /  \
      5    15
     / \
    2   7
```

### Questions

1. What is the root node?
2. Which nodes are leaves?
3. What is the preorder traversal?
4. What is the inorder traversal?
5. How does this tree differ from a general graph?

### Expected Answers

1. The root is 10.
2. The leaves are 2, 7, and 15.
3. Preorder: 10, 5, 2, 7, 15.
4. Inorder: 2, 5, 7, 10, 15.
5. This tree is connected and has no cycles, with a clear parent-child hierarchy. A general graph may contain cycles, may be disconnected, and does not require a root.

## 9. Why Non-Linear Data Structures Matter

Non-linear data structures are essential when information contains hierarchical relationships or complex networks. Trees organize information into levels and can support efficient search operations when appropriately structured. Graphs represent interconnected systems and support pathfinding and network analysis.

These structures are also important in artificial intelligence and computing applications, including decision trees, knowledge graphs, recommendation systems, and dependency analysis. Understanding their organization helps programmers choose suitable structures and algorithms for complex problems.

## References

1. OpenDSA. *Data Structures and Algorithms*. Virginia Tech. https://opendsa-server.cs.vt.edu/
2. Cormen, T. H., Leiserson, C. E., Rivest, R. L., and Stein, C. (2022). *Introduction to Algorithms* (4th ed.). MIT Press.
3. VisuAlgo. *Data Structures and Algorithms Visualizations*. https://visualgo.net/en
