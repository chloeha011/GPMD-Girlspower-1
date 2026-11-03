# Non-Linear Data Structures

## 1. Definition

A non-linear data structure organizes data in a hierarchical or network-like form rather than one single sequence. A node can connect to more than one other node, allowing the structure to represent branching relationships and multiple possible paths.

The two main types are **trees** and **graphs**. Trees represent hierarchical relationships, such as folders within a computer. Graphs represent general connections, such as roads between locations or relationships in a social network.

Unlike linear structures such as arrays, linked lists, stacks, and queues, non-linear structures are useful when data contains branching relationships or complex connections.

### Linear vs. Non-Linear Data Structures

- **Linear:** Elements follow one logical sequence. Examples include arrays, linked lists, stacks, and queues.
- **Non-linear:** Elements have branching or network-like connections. Examples include trees and graphs.

## 2. How Non-Linear Data Structures Work

Non-linear data structures are commonly described using **nodes** and **connections**.

- **Node:** An individual unit that stores data.
- **Edge:** A connection between two nodes. In a tree, edges usually represent parent-child relationships.

A program starts from a chosen node, such as the root of a tree or a starting vertex in a graph, and follows connections using a traversal or search algorithm.

### General Process

1. Create nodes to store individual data elements.
2. Connect nodes according to the relationships being represented.
3. Choose a starting node when an operation requires one.
4. Traverse or search the structure using a suitable algorithm.
5. Add, remove, or update nodes and connections when the data changes.

### Memory Organization

Non-linear structures can be stored in different ways:

- **Linked representation:** Nodes store references to other nodes. This is common in trees and adjacency-list graphs.
- **Array-based representation:** Values or nodes are stored in arrays and related through index positions. Binary heaps are commonly implemented this way.
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

A **tree** is a hierarchical data structure made of nodes connected by edges. A rooted tree has one starting node called the **root**. Other nodes are arranged in parent-child relationships.

A conventional tree with \(n\) nodes has exactly \(n-1\) edges. A tree is connected and contains no cycles.

### Example of a Tree

\`\`\`
        A
       / \\
      B   C
     / \\ / \\
    D  E F  G
\`\`\`

A is the root. B and C are its children. D, E, F, and G are leaf nodes.

**Important terminology**

- **Root:** The topmost node of a rooted tree.
- **Parent:** A node that has one or more child nodes.
- **Child:** A node directly connected below another node.
- **Leaf:** A node with no children.
- **Edge:** A connection between two nodes.
- **Subtree:** A node together with its descendants.
- **Depth:** The number of edges from the root to a particular node.
- **Height:** The number of edges on the longest downward path from a node to a leaf.

**How a tree works**

1. Data is stored in nodes.
2. A root node provides the starting point.
3. Other nodes are connected through parent-child relationships.
4. A traversal algorithm visits nodes in a defined order.
5. Search and insertion operations follow the rules of the particular tree type.

**Common types of trees**

- **Binary tree:** Each node has at most two children.
- **Binary search tree (BST):** For each node, values in the left subtree are smaller and values in the right subtree are larger, assuming distinct keys and the standard ordering rule.
- **Heap:** A complete binary tree that follows a heap-order rule. In a max-heap, each parent is greater than or equal to its children; in a min-heap, each parent is less than or equal to its children.
- **Trie:** A tree-like structure used to store sequences, often words, by shared prefixes.

**Advantages**

- Represents hierarchical relationships naturally.
- Some types, such as balanced search trees, support efficient searching and insertion.
- Organizes information into clear levels.

**Limitations**

- More complex to implement than basic linear structures.
- An unbalanced binary search tree can become inefficient.
- Traversal and memory management may require additional logic.

**Common applications**

- Computer file systems.
- Organizational charts.
- Database indexing.
- Search operations.
- Autocomplete and word prediction.

### 4.2 Graphs

A **graph** is a non-linear data structure consisting of **vertices** (also called nodes) and **edges** that connect pairs of vertices. Unlike a tree, a graph does not need to follow a hierarchy. It may contain cycles, and a vertex can connect to many others.

A graph is commonly represented as:

\[
G=(V,E)
\]

where:

- \(V\) is the set of vertices.
- \(E\) is the set of edges connecting vertices.

### Example of a Graph

\`\`\`
A ----- B
|       |
|       |
C ----- D
\`\`\`

Each letter represents a vertex, and each line represents an edge.

**Important terminology**

- **Vertex:** An individual node in a graph.
- **Edge:** A connection between two vertices.
- **Adjacent vertices:** Vertices directly connected by an edge.
- **Degree:** The number of edges connected to a vertex in an undirected graph.
- **Path:** A sequence of vertices connected by edges.
- **Cycle:** A path that starts and ends at the same vertex.
- **Weight:** A value assigned to an edge, such as distance, cost, or time.

**How a graph works**

1. Define vertices to represent objects or entities.
2. Create edges to represent relationships between them.
3. Store the connections using an adjacency list or adjacency matrix.
4. Use algorithms to explore the graph, find paths, or identify relationships.
5. Update vertices, edges, or weights when the network changes.

**Common types of graphs**

- **Undirected graph:** Edges have no direction; a connection works both ways.
- **Directed graph:** Edges have a direction, such as \(A \rightarrow B\).
- **Weighted graph:** Edges have values such as cost, distance, or time.
- **Unweighted graph:** Edges represent connections without assigned weights.
- **Cyclic graph:** Contains at least one cycle.
- **Acyclic graph:** Contains no cycles. A directed acyclic graph (DAG) is useful for representing dependencies.

**Advantages**

- Represents complex relationships naturally.
- Supports pathfinding and network analysis.
- Models interconnected systems in many real-world situations.

**Limitations**

- Dense graphs can require substantial memory.
- Searching and traversal can become expensive for large networks.
- Some graph problems require complex algorithms.

**Common applications**

- Social networks.
- Road and transportation networks.
- Computer networks.
- Recommendation systems.
- Project scheduling and dependency management.
- Knowledge representation in artificial intelligence.

## 5. Comparison of Trees and Graphs

| Feature | Tree | Graph |
| --- | --- | --- |
| Organization | Hierarchical | Network-like |
| Connections | Parent-child relationships | General vertex-to-vertex relationships |
| Root | A rooted tree has one root | No root is required |
| Cycles | No cycles | May contain cycles |
| Connectivity | Connected by definition | May be connected or disconnected |
| Number of edges | A tree with \(n\) nodes has \(n-1\) edges | Depends on the graph |
| Common applications | File systems, search trees | Social networks, routes, dependencies |

## 6. Traversal of Non-Linear Data Structures

**Traversal** is the process of visiting nodes to inspect or process their data. The order depends on the chosen algorithm.

### 6.1 Graph Traversal

Two widely used graph traversal algorithms are:

- **Breadth-First Search (BFS):** Visits nearby nodes first, exploring the graph level by level. It typically uses a queue.
- **Depth-First Search (DFS):** Follows one path as far as possible before returning to explore another path. It typically uses a stack or recursion.

For an unweighted graph, BFS can find a shortest path measured by the number of edges, provided the search begins at the source vertex.

### 6.2 Tree Traversal

Common traversal methods for binary trees include:

- **Preorder:** Visit the root, then the left subtree, then the right subtree.
- **Inorder:** Visit the left subtree, then the root, then the right subtree.
- **Postorder:** Visit the left subtree, then the right subtree, then the root.
- **Level-order:** Visit nodes level by level, typically using a queue.

The choice of traversal depends on the task. For example, inorder traversal of a binary search tree visits values in sorted order when the tree follows the standard BST ordering rule.

### 6.3 Time Complexity of Traversal

Time complexity describes how the time required by an algorithm changes as the amount of data increases.

For BFS and DFS, the typical time complexity using an adjacency-list representation is \(O(V+E)\), where:

- \(V\) represents the number of vertices.
- \(E\) represents the number of edges.

This means the algorithm processes each vertex and edge a limited number of times.

For tree traversal, the time complexity is \(O(n)\), where \(n\) is the number of nodes, because each node is visited once.

## 7. Basic Performance of Tree Operations

The performance of tree operations depends on the type and structure of the tree.

For a **binary search tree (BST)**:

- **Searching:** Typically \(O(\log n)\) when the tree is balanced.
- **Insertion:** Typically \(O(\log n)\) when the tree is balanced.
- **Deletion:** Typically \(O(\log n)\) when the tree is balanced.

However, if the tree becomes highly unbalanced, these operations can take \(O(n)\) time in the worst case.

A balanced tree keeps its height relatively small, allowing operations to reach the required nodes more quickly.

## 8. Worked Example: Finding a Path in a Graph

Suppose a small transport network has four locations connected as follows:

- A connects to B and C.
- B connects to D.
- C connects to D.

The connections can be shown as:

\`\`\`
    B
   / \\
  A   D
   \\ /
    C
\`\`\`

**Task:** Find a path from A to D using BFS, exploring B before C.

1. Start at A. Add its unvisited neighbors B and C to the queue.  
   Queue: \`[B, C]\`
2. Visit B. Its neighbor D has not been discovered, so add D.  
   Queue: \`[C, D]\`
3. Visit C. D has already been discovered, so do not add it again.  
   Queue: \`[D]\`
4. Visit D. The target has been found.

**Expected result:** One shortest path is \`A → B → D\`, containing two edges. The alternative path \`A → C → D\` is also shortest because it contains two edges.

This example shows how BFS uses a queue to explore a graph level by level and find a shortest path in an unweighted graph.

## 9. Learner Activity

Consider the following tree:

\`\`\`
        10
       /  \\
      5    15
     / \\
    2   7
\`\`\`

**Questions**

1. What is the root node?
2. Which nodes are leaves?
3. What is the preorder traversal?
4. How does this tree differ from a general graph?

### Expected Answers

1. The root is 10.
2. The leaves are 2, 7, and 15.
3. Preorder traversal: 10, 5, 2, 7, 15.
4. A tree is a connected, acyclic hierarchical structure. A general graph may contain cycles, may be disconnected, and does not require a root.

## 10. Why Non-Linear Data Structures Matter

Non-linear data structures are important when information contains hierarchical relationships or complex networks. Trees organize data into levels and can support efficient search operations when appropriately structured. Graphs represent interconnected systems and support tasks such as pathfinding and network analysis.

These structures are also used in artificial intelligence, including decision trees, knowledge graphs, and search algorithms. Understanding trees and graphs helps programmers choose suitable ways to represent and process complex relationships.

## References

1. OpenDSA. *Data Structures and Algorithms*. Virginia Tech. https://opendsa-server.cs.vt.edu/
2. Cormen, T. H., Leiserson, C. E., Rivest, R. L., and Stein, C. *Introduction to Algorithms* (4th ed.). MIT Press, 2022.
3. VisuAlgo. *Data Structures and Algorithms Visualizations*. https://visualgo.net/en
