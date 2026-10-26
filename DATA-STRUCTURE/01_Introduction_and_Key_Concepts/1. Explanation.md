
# Data Structures

## 1. Introduction to Data Structures

### 1.1 What Is a Data Structure?

A data structure is a way of organizing and storing data in a computer so that it can be accessed, changed, and used efficiently.

Computers work with large amounts of information. For example, a university system may store student names, identification numbers, grades, and course information. If this information is not organized properly, it can become difficult to find or update the information we need.

Data structures help solve this problem by arranging information in different ways depending on how it will be used.

We can understand this idea through an everyday example.

Imagine that you have 20 books. You could put all of them in one large box. The books would be stored, but finding a particular book might take a long time.

Instead, you could organize them by subject, arrange them alphabetically, or place frequently used books on a separate shelf. Each method makes it easier to find certain books.

Computers use a similar principle. A data structure provides an organized way to store information so that different operations can be performed on it.

### 1.2 Why Are Data Structures Important?

Data structures are important because they affect how efficiently a program can work with information.

Programs often need to perform several common operations:

- **Access:** Get a particular piece of data.
- **Search:** Find an item in a collection.
- **Insert:** Add a new item.
- **Delete:** Remove an item.
- **Update:** Change existing information.
- **Traverse:** Visit the items in a collection, often one by one.

Different data structures make these operations easier or more efficient in different situations.

For example, imagine an application that stores a student's grades. The application may need to display all grades, find the highest grade, add a new result, or update an existing grade. The way the grades are organized affects how these tasks are performed.

There is no single data structure that is best for every situation. The most suitable choice depends on the type of information and the operations a program needs to perform.

### 1.3 The Relationship Between Data Structures and Algorithms

Data structures and algorithms are closely connected, but they have different purposes.

A data structure determines how information is organized and stored. An algorithm describes the steps used to solve a problem or perform a task.

Consider a university database containing student names.

- The data structure stores the names in an organized form.
- A searching algorithm explains how to find a particular name.
- A sorting algorithm explains how to arrange the names alphabetically.

The data structure and algorithm work together to solve the problem.

Choosing an appropriate data structure can also make an algorithm more efficient. For example, finding an item in a well-organized structure may require fewer steps than searching through an unorganized collection.

## 2. Common Types of Data Structures

Data structures can organize information in several ways. Some store items in a sequence, while others organize items according to relationships or connections.

This section introduces six important examples:

1. Arrays
2. Linked lists
3. Stacks
4. Queues
5. Trees
6. Graphs

Each structure has its own characteristics and is useful for different types of tasks.

### 2.1 Arrays

An array is a data structure that stores a sequence of elements. Each element has a position, often called an **index**, that can be used to access it.

For example, imagine that a teacher wants to store the grades of five students.

The grades could be represented as follows:

```text
[85, 92, 78, 90, 88]
```

Each number represents one student's grade.

In many programming languages, the first element has index `0`, the second has index `1`, and so on.

| Index | Grade |
|---:|---:|
| 0 | 85 |
| 1 | 92 |
| 2 | 78 |
| 3 | 90 |
| 4 | 88 |

If we want to access the grade at index `2`, we get `78`.

The exact rules for arrays depend on the programming language. Some arrays have a fixed size, while other array-like structures can grow or shrink.

**How do arrays work?**

Imagine that each element has its own numbered position. If you know the index, you can usually access the corresponding element directly.

For example, consider the array:

```text
["Apple", "Banana", "Orange", "Grape"]
```

If we want to access `"Orange"`, we use index `2` in a zero-based indexing system.

This makes arrays convenient when we need to access items by position.

**Advantages of arrays**

- Elements can usually be accessed quickly by index.
- The elements are organized in a clear sequence.
- Arrays are useful for storing lists of similar kinds of information, such as grades, prices, or temperatures.

**Disadvantages of arrays**

- Inserting or deleting an element in the middle may require other elements to shift.
- Fixed-size arrays cannot grow beyond their allocated capacity.
- Finding a particular value may still require searching through the elements if its position is unknown.

**When are arrays useful?**

Arrays are useful when data needs to be stored in a sequence and accessed by position. Examples include storing monthly sales figures, examination results, or daily temperatures.

### 2.2 Linked Lists

A linked list is a data structure made up of elements called **nodes**. Each node stores data and a reference to another node, which connects the elements together.

Unlike an array, a linked list does not rely on elements being stored as one indexed sequence. Instead, each node contains information about where the next node can be found.

For example, imagine a list of tasks:

```text
Task A → Task B → Task C → Task D
```

Each task represents a node. The arrow shows that one node points to the next node.

A simple linked list usually has a starting node, called the **head**. To reach a later node, we follow the links from the beginning.

**How does a linked list work?**

Suppose we have the following linked list:

```text
10 → 20 → 30 → 40 → NULL
```

Each node contains a value and a reference to the next node.

- The first node stores `10` and links to the node containing `20`.
- The second node stores `20` and links to the node containing `30`.
- The third node stores `30` and links to the node containing `40`.
- The final node stores `40` and has no next node, represented here by `NULL`.

The exact representation depends on the programming language, but the main idea is that nodes are connected through references.

**Advantages of linked lists**

- They can grow or shrink as elements are added or removed.
- Inserting or deleting a node can be efficient when the relevant position or node is already known.
- They do not require all elements to be stored in one continuous block of memory.

**Disadvantages of linked lists**

- Accessing an element by position usually requires moving through the list from the beginning.
- Each node needs additional memory for its references.
- Managing links can make implementation more complicated than using an array.

**When are linked lists useful?**

Linked lists can be useful when a program frequently inserts or removes elements at known positions. They are also helpful for understanding how more complex data structures can be built from connected nodes.

However, linked lists are not automatically better than arrays. For example, arrays are generally more convenient when fast access by index is important.

### 2.3 Stacks

A stack is a data structure that follows the principle **Last In, First Out (LIFO)**.

This means that the last item added is the first item removed.

Think of a stack of plates. When you place a new plate on top, it becomes the first plate you can take away. To reach a plate underneath, you usually need to remove the plates above it first.

**How does a stack work?**

Imagine an empty stack.

1. Add `10`.
2. Add `20`.
3. Add `30`.

The stack now looks like this:

```text
Top
 ↓
[30]
[20]
[10]
```

If we remove one item, the value `30` is removed first because it was added most recently.

The remaining stack is:

```text
Top
 ↓
[20]
[10]
```

Stacks commonly support three operations:

- **Push:** Add an item to the top.
- **Pop:** Remove the top item.
- **Peek:** View the top item without removing it.

In a typical stack implementation, adding and removing the top item can be performed efficiently.

**Advantages of stacks**

- Their rules are simple and easy to understand.
- Adding or removing the top element is usually efficient.
- They are useful whenever the most recent item needs to be handled first.

**Disadvantages of stacks**

- Only the top item is directly available through standard stack operations.
- Accessing an item lower down usually requires removing items above it or using another method.

**When are stacks useful?**

Stacks are used in many computer applications. For example:

- **Undo operations:** A text editor can store recent actions so that the latest action can be undone first.
- **Browser history:** A stack-like approach can support certain navigation operations.
- **Function calls:** Programs use a call stack to keep track of active function calls.

The key idea is that a stack processes the most recently added item first.

### 2.4 Queues

A queue is a data structure that usually follows the principle **First In, First Out (FIFO)**.

This means that the first item added is the first item removed.

A queue works like a line of people waiting to buy tickets. The person who arrives first is normally served first, while new arrivals join the end of the line.

**How does a queue work?**

Imagine a queue containing three tasks:

```text
Front → [Task A] [Task B] [Task C] ← Rear
```

Task A is at the front, so it will be processed first.

Suppose a new task, Task D, arrives. It is added to the rear:

```text
Front → [Task A] [Task B] [Task C] [Task D] ← Rear
```

If Task A is processed and removed, Task B becomes the next item to be processed.

Queues commonly support two operations:

- **Enqueue:** Add an item to the rear of the queue.
- **Dequeue:** Remove an item from the front of the queue.

**Advantages of queues**

- They process items in the order they arrive.
- They are useful for managing tasks that must wait their turn.
- They help organize processes that share a limited resource.

**Disadvantages of queues**

- In a standard queue, items in the middle are not directly removed before items ahead of them.
- A queue may not be suitable when the newest item or the highest-priority item should be processed first.

**When are queues useful?**

Queues are useful in many everyday computer systems:

- Managing print jobs sent to a printer.
- Organizing customer requests on a server.
- Processing messages in the order they arrive.
- Managing tasks that are waiting to be executed.

The main difference between a stack and a queue is the order in which items are removed. A stack removes the most recently added item, while a queue normally removes the earliest added item.

### 2.5 Trees

A tree is a data structure that organizes data in a hierarchy. It consists of nodes connected by relationships, usually described as parent-child relationships.

Trees are similar to a family tree or the folders on a computer. A main folder can contain subfolders, and those subfolders can contain more folders or files.

**Basic tree terminology**

Consider this simple tree:

```text
       A
      / \
     B   C
    / \
   D   E
```

This structure contains several important concepts:

- **Root:** The top node. In this example, `A` is the root.
- **Parent:** A node that has one or more child nodes. For example, `B` is the parent of `D` and `E`.
- **Child:** A node directly connected below another node. For example, `C` is a child of `A`.
- **Leaf:** A node with no children. In this example, `C`, `D`, and `E` are leaves.
- **Edge:** A connection between two nodes.

A tree does not need to have exactly two children per node. The example above is a simple binary tree because each node has at most two children.

**How do trees work?**

Trees organize information according to relationships rather than simply placing everything in one sequence.

For example, a computer's file system can be represented as a tree:

```text
Documents
├── University
│   ├── Notes
│   └── Assignments
└── Personal
    ├── Photos
    └── Letters
```

The `Documents` folder is the root of this example. It contains two subfolders, and each of those folders can contain other items.

This hierarchical organization makes it easier to understand how information is grouped and to navigate between folders.

Some trees, such as binary search trees, also follow rules that help programs search for information efficiently. However, not every tree has these ordering rules.

**Advantages of trees**

- They represent hierarchical relationships clearly.
- They are useful for organizing data into levels.
- Certain tree structures support efficient searching, insertion, and deletion.

**Disadvantages of trees**

- They can be more complicated to implement and manage than simple lists.
- The efficiency of operations depends on the type and shape of the tree.
- An unbalanced search tree can become inefficient for some operations.

**When are trees useful?**

Trees are used in:

- Computer file systems.
- Organization charts.
- Family trees.
- Hierarchical menus.
- Search structures in databases and programs.

The main idea is that trees are useful when information naturally forms a hierarchy.

### 2.6 Graphs

A graph is a data structure used to represent objects and the relationships or connections between them.

A graph consists of two basic components:

- **Vertices (or nodes):** The objects being represented.
- **Edges:** The connections between those objects.

Graphs are especially useful for representing networks, where one object can be connected to many others.

**How do graphs work?**

Imagine a social network with four people: Anna, Ben, Chloe, and David.

Suppose the connections are:

- Anna is connected to Ben.
- Anna is connected to Chloe.
- Ben is connected to David.
- Chloe is connected to David.

We can represent these relationships as a graph:

```text
Anna ─── Ben
  |       |
  |       |
Chloe ─ David
```

Each person's name represents a vertex, and each line represents a connection between two people.

The diagram is a simplified illustration of the relationships. The connections do not necessarily represent real friendship rules or the direction of an interaction.

Graphs can be **undirected** or **directed**.

- **Undirected graph:** A connection works in both directions. For example, if two people are connected as friends, the relationship may be represented by an undirected edge.
- **Directed graph:** Connections have a direction. For example, if one social media user follows another, the connection goes from the follower to the account being followed.

Graphs can also be **weighted**. A weight is a value assigned to an edge, such as the distance between two cities or the cost of travelling between locations.

**Advantages of graphs**

- They represent complex relationships between objects.
- They can model networks and routes.
- They support algorithms for finding paths, exploring connections, and analyzing networks.

**Disadvantages of graphs**

- Large graphs can be complicated to store and process.
- Finding useful paths or analyzing relationships may require complex algorithms.
- Some graph problems become computationally expensive as the number of vertices and edges grows.

**When are graphs useful?**

Graphs are used in many real-world systems:

- **Navigation apps:** Cities or locations are represented as vertices, while roads are represented as edges.
- **Social networks:** Users are vertices, and relationships are edges.
- **Computer networks:** Devices are vertices, and communication links are edges.
- **Recommendation systems:** Connections can represent relationships between users, products, or interests.

The main idea is that graphs are suitable when the connections between items are as important as the items themselves.

## 3. Comparing Different Data Structures

Each data structure organizes information differently. Understanding these differences helps programmers choose a suitable structure for a problem.

| Data structure | How data is organized | Main advantage | Example use |
|---|---|---|---|
| Array | Elements arranged in a sequence with positions | Fast access by index | Student grades |
| Linked list | Nodes connected by references | Flexible insertion and deletion at known positions | A sequence of changing items |
| Stack | Items added and removed at the top | Processes the newest item first | Undo operations |
| Queue | Items added at the rear and removed at the front | Processes items in arrival order | Print jobs |
| Tree | Nodes organized hierarchically | Represents parent-child relationships | File systems |
| Graph | Nodes connected by edges | Represents networks and relationships | Maps and social networks |

These are general descriptions rather than guarantees about performance. The efficiency of an operation can depend on the specific implementation and the way the data is used.

## 4. How Do We Choose a Data Structure?

When choosing a data structure, a programmer should first consider what the program needs to do.

For example:

- If a program needs to access elements frequently by their position, an array may be suitable.
- If a program needs to process the newest item first, a stack may be appropriate.
- If a program needs to process items in the order they arrive, a queue may be appropriate.
- If a program needs to represent hierarchical information, a tree may be useful.
- If a program needs to represent relationships between many connected objects, a graph may be the best choice.

There are often several possible solutions to the same problem. The goal is to select a structure that makes the required operations convenient and efficient.

### Example: Designing a University Application

Imagine that we are developing an application for university students.

Different parts of the application may use different data structures:

- **Grades:** An array could store a sequence of grades.
- **Undoing edits:** A stack could keep track of recent actions.
- **Pending requests:** A queue could process requests in arrival order.
- **University departments:** A tree could represent departments and their subgroups.
- **Connections between students:** A graph could represent relationships within a student network.

This example demonstrates that one application can use several data structures because different tasks have different requirements.

## Sources

1. **MIT OpenCourseWare — Introduction to Algorithms (Spring 2020)**  
   A university-level course with lecture notes on data structures, hashing, binary trees, heaps, and related algorithms. Some material is more advanced than this beginner introduction.  
   https://ocw.mit.edu/courses/6-006-introduction-to-algorithms-spring-2020/pages/lecture-notes/

2. **Brooklyn College — CISC 3130 Data Structures**  
   An educational resource covering arrays, linked lists, stacks, queues, trees, graphs, and other data structures.  
   https://libguides.brooklyn.cuny.edu/cisc3130/schedule

3. **Universidad Carlos III de Madrid — Data Structures and Algorithms Lecture Notes**  
   University teaching materials covering abstract data types, stacks, queues, linked lists, binary search trees, and graphs.  
   https://ocw.uc3m.es/mod/page/view.php?id=3160&lang=en

4. **University of Michigan — EECS 281 Lecture Notes**  
   Course notes covering data structures and algorithms, including arrays, lists, stacks, queues, trees, and graphs.  
   https://www.eecs.umich.edu/courses/eecs281/f04/lecnotes.html
