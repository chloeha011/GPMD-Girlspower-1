# Data Structures: Introduction and Key Concepts

## 1. Introduction to Data Structures

### 1.1 What Is a Data Structure?

A **data structure** is a way of organizing and storing data so that a computer program can access, update, and process it.

Programs often work with many kinds of information. For example, a university system may store student names, identification numbers, grades, and course details. Organizing this information makes it easier to find and manage what the program needs.

Think of having 20 books. You could place them all in one box, but finding a particular book might take time. If you arrange them by subject or title, finding one becomes easier. Data structures apply a similar idea to information used by computer programs.

Different data structures organize data in different ways. The best choice depends on what the program needs to do with the data.

### 1.2 Why Are Data Structures Important?

A program may need to perform several common operations on stored data:

- **Access:** Retrieve an item from a particular position or location.
- **Search:** Find an item that matches a value or condition.
- **Insert:** Add a new item.
- **Delete:** Remove an item.
- **Update:** Change an existing item.
- **Traverse:** Visit the items in a data structure, usually in a particular order.

Different data structures support these operations in different ways. For example, an array allows direct access by index, while a linked list usually requires moving through nodes to reach an item by position.

There is no single data structure that is best for every task. Programmers choose one based on the type of data, the operations required, and the efficiency needed.

### 1.3 Data Structures and Algorithms

A **data structure** organizes and stores information. An **algorithm** is a set of steps used to solve a problem or complete a task.

They work together. For example, a program might store student names in an array and use a searching algorithm to find a particular name. It could use a sorting algorithm to arrange the names alphabetically.

Choosing a suitable data structure can make an algorithm easier to implement or more efficient. In the same way, the algorithm chosen affects how the data structure is used.

## 2. Common Types of Data Structures

Data structures can be grouped in different ways. One useful distinction is between **linear** and **non-linear** structures:

- **Linear data structures** arrange elements in a sequence. Examples include arrays, linked lists, stacks, and queues.
- **Non-linear data structures** organize elements in hierarchical or network-like relationships. Examples include trees and graphs.

The following sections introduce six commonly used structures.

### 2.1 Arrays

An **array** stores elements in an ordered sequence. Each element can be accessed using its **index**, which identifies its position.

For example, a teacher could store five students' grades in an array:

```text
[85, 92, 78, 90, 88]
```

In a zero-based indexing system, the first element has index `0`, the second has index `1`, and so on.

| Index | Grade |
|---:|---:|
| 0 | 85 |
| 1 | 92 |
| 2 | 78 |
| 3 | 90 |
| 4 | 88 |

The grade at index `2` is `78`.

**How it works:** Each element has a position in the sequence. If the index is known, a program can usually access the corresponding element directly.

**Advantages**
- Fast access to an element by index.
- Simple way to store and process an ordered collection.
- Useful when the number of items is known or when access by position is common.

**Limitations**
- Inserting or deleting an element in the middle may require other elements to shift.
- Some arrays have a fixed capacity. Dynamic array structures can grow, but resizing may require additional work.
- Finding a value when its position is unknown may require a search.

**Common uses:** Storing grades, temperatures, prices, or other ordered collections.

### 2.2 Linked Lists

A **linked list** is a sequence of **nodes**. Each node stores data and a reference to another node. In a singly linked list, each node refers to the next node.

Example:

```text
10 → 20 → 30 → 40 → NULL
```

The first node is called the **head**. Each arrow represents a link to the next node. `NULL` indicates that the final node has no next node.

**How it works:** To reach a particular node, a program follows the links from the head until it reaches the required node. Unlike an array, a linked list does not provide direct access by index.

**Advantages**
- Can grow or shrink as nodes are added or removed.
- Insertion or deletion can be efficient when the relevant node or its preceding node is already known.
- Nodes do not need to be stored next to one another in memory.

**Limitations**
- Accessing a node by position usually requires moving through the list from the head.
- Each node needs extra memory for its link or links.
- Managing connections between nodes can make implementation more complex.

**Common uses:** Implementing other data structures and managing collections where items are frequently inserted or removed at known positions.

**Important:** Linked lists are not always better than arrays. Arrays are generally more suitable when frequent access by index is needed.

### 2.3 Stacks

A **stack** is a data structure that follows the **Last In, First Out (LIFO)** principle: the most recently added item is the first one removed.

Think of a stack of plates. A new plate is placed on top, and the top plate is normally the first one taken off.

Example: after pushing `10`, `20`, and `30` onto an empty stack:

```text
Top
 ↓
[30]
[20]
[10]
```

The next item removed is `30`, because it was added last.

**Main operations**
- **Push:** Add an item to the top.
- **Pop:** Remove the item at the top.
- **Peek (or Top):** View the top item without removing it.

**Advantages**
- Simple rules for adding and removing items.
- Adding or removing the top item is usually efficient.
- Useful when the most recent item must be handled first.

**Limitations**
- Standard stack operations provide access to the top item only.
- Reaching an item lower in the stack requires removing the items above it or using another method.

**Common uses:** Undo features, function-call management, and checking matching brackets in expressions.

### 2.4 Queues

A **queue** is a data structure that usually follows the **First In, First Out (FIFO)** principle: the earliest added item is the first one removed.

A queue works like a line of people waiting for a service. New arrivals join the rear, and the person at the front is served first.

Example:

```text
Front → [Task A] [Task B] [Task C] ← Rear
```

If Task A is removed, Task B becomes the next item at the front.

**Main operations**
- **Enqueue:** Add an item to the rear.
- **Dequeue:** Remove an item from the front.
- **Front (or Peek):** View the item at the front without removing it.

**Advantages**
- Processes items in arrival order.
- Useful for managing tasks waiting for a shared resource.
- Helps organize requests that should be handled in sequence.

**Limitations**
- In a standard queue, an item cannot normally be removed from the middle before the items ahead of it.
- A basic FIFO queue is not suitable when tasks must be processed by priority.

**Common uses:** Print jobs, waiting requests on a server, and task scheduling.

**Stack vs. queue:** A stack removes the most recently added item (LIFO), while a queue removes the earliest added item (FIFO).

### 2.5 Trees

A **tree** is a non-linear data structure that organizes data hierarchically. It consists of nodes connected by edges and commonly uses parent-child relationships.

Example:

```text
       A
      / \\
     B   C
    / \\
   D   E
```

**Basic terminology**
- **Root:** The top node of a rooted tree. In this example, `A` is the root.
- **Parent:** A node directly above one or more child nodes. `B` is the parent of `D` and `E`.
- **Child:** A node directly below its parent. `C` is a child of `A`.
- **Leaf:** A node with no children. Here, `C`, `D`, and `E` are leaves.
- **Edge:** A connection between two nodes.

A **binary tree** is a tree in which each node has at most two children. Not all trees are binary trees.

**How it works:** Nodes are connected according to their hierarchical relationships. A program can follow these connections to find, add, remove, or visit nodes. Some types of trees follow additional rules to make searching more efficient.

**Advantages**
- Represents hierarchical information clearly.
- Organizes data into levels and relationships.
- Certain types, such as balanced search trees, support efficient searching and updating.

**Limitations**
- More complex to implement than a simple array or list.
- Performance depends on the type and shape of the tree.
- An unbalanced search tree may make some operations slower.

**Common uses:** Computer folder systems, organization charts, hierarchical menus, and search structures.

### 2.6 Graphs

A **graph** is a non-linear data structure used to represent objects and the connections between them. It consists of **vertices** (also called nodes) and **edges** that connect pairs of vertices.

For example, a simplified network of four people could be represented as:

```text
Anna ─── Ben
  |       |
  |       |
Chloe ─ David
```

Each name represents a vertex, and each line represents an edge. The diagram shows connections only; it does not specify what those relationships mean.

**Common graph types**
- **Undirected graph:** Edges have no direction. A connection is represented as going both ways.
- **Directed graph:** Edges have a direction, showing which vertex the connection goes from and to.
- **Weighted graph:** Edges have numerical values, such as distance, time, or cost.

**How it works:** A program stores vertices and the edges between them. It can then explore connections, find paths, or analyze relationships using graph algorithms.

**Advantages**
- Represents complex relationships and networks.
- Models routes and connections between many objects.
- Supports tasks such as pathfinding and network analysis.

**Limitations**
- Large graphs can require significant memory and processing.
- Finding paths or analyzing relationships may require more complex algorithms.
- Performance depends on the graph's size, connections, and representation.

**Common uses:** Navigation systems, social networks, computer networks, and recommendation systems.

**Tree vs. graph:** A tree is a connected structure with no cycles and a hierarchical organization. A general graph can have cycles, may be disconnected, and does not need a root.

## 3. Comparing the Six Data Structures

| Data structure | How data is organized | Useful when... | Example use |
|---|---|---|---|
| Array | Ordered elements accessed by index | Access by position is important | Student grades |
| Linked list | Nodes connected by references | Items are inserted or removed at known locations | A changing sequence of items |
| Stack | Items added and removed at the top | The latest item should be handled first | Undo operations |
| Queue | Items added at the rear and removed at the front | Items should be handled in arrival order | Print jobs |
| Tree | Nodes arranged hierarchically | Data has parent-child relationships | File systems |
| Graph | Vertices connected by edges | Relationships or routes between items matter | Maps and social networks |

These are general characteristics, not guarantees about speed. The performance of an operation depends on the specific implementation and the amount and arrangement of data.

## 4. Choosing a Suitable Data Structure

When choosing a data structure, a programmer should consider:

1. **The type of data:** What information needs to be stored?
2. **Required operations:** Will the program search, access, insert, delete, or update items frequently?
3. **Efficiency:** How much time and memory can the program use?
4. **Relationships:** Is the information arranged in a sequence, hierarchy, or network?

For example:
- Use an **array** when frequent access by position is needed.
- Use a **stack** when the most recently added item should be processed first.
- Use a **queue** when items should be processed in arrival order.
- Use a **tree** when information has a hierarchical structure.
- Use a **graph** when the connections between items are important.

### Example: A University Application

A university application may use several data structures because its features have different requirements:

- **Grades:** An array can store a sequence of grades.
- **Undoing edits:** A stack can keep track of recent actions.
- **Pending requests:** A queue can process requests in arrival order.
- **Departments:** A tree can represent departments and their subgroups.
- **Student connections:** A graph can represent relationships in a student network.

This example shows that a single program can use multiple data structures. The appropriate choice depends on the task each part of the program needs to perform.

## Sources

1. **MIT OpenCourseWare — Introduction to Algorithms (Spring 2020).** University lecture notes covering data structures and related algorithms. Some topics are more advanced than this introductory chapter.  
   https://ocw.mit.edu/courses/6-006-introduction-to-algorithms-spring-2020/pages/lecture-notes/

2. **Brooklyn College — CISC 3130: Data Structures.** Course materials covering common data structures, including arrays, linked lists, stacks, queues, trees, and graphs.  
   https://libguides.brooklyn.cuny.edu/cisc3130/schedule

3. **Universidad Carlos III de Madrid — Data Structures and Algorithms Lecture Notes.** University materials covering abstract data types and common data structures.  
   https://ocw.uc3m.es/mod/page/view.php?id=3160&lang=en

4. **University of Michigan — EECS 281 Lecture Notes.** Course notes on data structures and algorithms.  
   https://www.eecs.umich.edu/courses/eecs281/f04/lecnotes.html
