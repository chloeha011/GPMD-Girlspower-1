# Terminology: Data Structures

This glossary explains important terms used in data structures. Definitions are written for beginners and use consistent terminology across arrays, linked lists, stacks, queues, trees, graphs, and hash tables.

## 1. Data Structure

A **data structure** is a way of organizing and storing data so that a computer program can access, update, and process it.

**Example:** A program may store student records in an array or use a hash table to look up a student by ID.

## 2. Data Element

A **data element** (often shortened to *element*) is an individual item stored in a data structure.

**Example:** In the array `[5, 10, 15]`, each number is an element.

## 3. Array

An **array** is an ordered collection of elements. Each element is identified by an index, which allows it to be accessed directly by its position.

**Example:** In `[10, 20, 30, 40]`, the element `30` is at index 2 in a zero-based indexing system.

**Note:** Many programming languages start array indexes at 0, but indexing rules depend on the language or data structure.

## 4. Index

An **index** is a number that identifies an element's position in an indexed data structure, such as an array.

**Example:** In `[10, 20, 30]`, the element `10` has index 0 in Python.

## 5. Linked List

A **linked list** is a sequence of nodes in which each node stores data and a reference to another node. In a singly linked list, each node refers to the next node; in a doubly linked list, each node can refer to both the next and previous nodes.

**Example:** A linked list of tasks can connect each task to the next task in the sequence.

## 6. Node

A **node** is an individual unit in a data structure. Depending on the structure, it may store data, references to other nodes, or both.

**Example:** A node in a singly linked list stores a value and a reference to the next node.

## 7. Pointer and Reference

A **pointer** is a value that stores a memory address. A **reference** provides a way to refer to another object or data item. The exact distinction depends on the programming language.

**Example:** A linked-list node may contain a pointer or reference to the next node.

**Note:** Not every programming language exposes pointers directly. For beginner-level explanations, the word *reference* is often more general.

## 8. Stack

A **stack** is a data structure that follows the **Last In, First Out (LIFO)** principle. The most recently added element is the first one removed.

- **Push:** Adds an element to the top of the stack.
- **Pop:** Removes the top element.
- **Peek/Top:** Views the top element without removing it.

**Example:** A stack of plates: the plate placed on top is usually the first one taken off.

## 9. Queue

A **queue** is a data structure that usually follows the **First In, First Out (FIFO)** principle. The earliest added element is the first one removed.

- **Enqueue:** Adds an element to the rear of the queue.
- **Dequeue:** Removes an element from the front of the queue.
- **Front/Head:** Refers to the element at the front.
- **Rear/Tail:** Refers to the end where new elements are added.

**Example:** People waiting in a line are generally served in the order they arrive.

## 10. Tree

A **tree** is a hierarchical data structure made up of nodes connected by edges. In a rooted tree, the top node is called the root, and the other nodes are arranged in parent-child relationships.

- **Root:** The node at the top of a rooted tree; it has no parent.
- **Parent:** A node directly above one or more child nodes.
- **Child:** A node directly below its parent.
- **Leaf:** A node with no children.
- **Edge:** A connection between two nodes.

**Example:** A computer's folder structure can be represented as a tree, with folders containing subfolders.

## 11. Graph

A **graph** is a data structure made up of vertices (also called nodes) and edges that connect them. Graphs represent relationships or connections between objects.

- **Vertex:** An individual point or node in a graph.
- **Edge:** A connection between two vertices.
- **Directed Graph:** A graph in which edges have a direction.
- **Undirected Graph:** A graph in which edges have no direction.
- **Weighted Graph:** A graph in which edges have numerical values, such as distance or cost.

**Example:** A social network can be represented as a graph, where people are vertices and their connections are edges.

## 12. Hash Table

A **hash table** is a data structure that stores information as key-value pairs. It uses a **hash function** to calculate where a key's value should be stored, helping the program find information efficiently.

- **Key:** The identifier used to look up a value.
- **Value:** The information associated with a key.
- **Hash Function:** A function that converts a key into a position or index in the hash table.
- **Collision:** Occurs when two different keys are mapped to the same position.

**Example:** A student ID can be used as a key to look up that student's record.

## 13. Traversal

**Traversal** is the process of visiting the elements or nodes in a data structure, usually in a particular order.

**Example:** Traversing an array means visiting its elements one by one. Tree and graph traversal use specific methods, such as depth-first search (DFS) or breadth-first search (BFS).

## 14. Searching

**Searching** is the process of finding a particular element or checking whether it exists in a data structure.

**Example:** Searching an array for the value `20` means checking the elements until `20` is found or the search is complete.

## 15. Insertion

**Insertion** is the operation of adding a new element to a data structure. The position of the new element depends on the structure and the insertion method.

**Example:** Inserting `25` before `30` in `[10, 20, 30]` produces `[10, 20, 25, 30]`.

## 16. Deletion

**Deletion** is the operation of removing an element from a data structure.

**Example:** Deleting `20` from `[10, 20, 30]` produces `[10, 30]`.

## 17. Time Complexity

**Time complexity** describes how the number of operations performed by an algorithm grows as the input size increases. It is commonly expressed using Big-O notation.

**Example:** A simple search through an unsorted array may need to check every element, so its worst-case time complexity is `O(n)`.

## 18. Space Complexity

**Space complexity** describes how the amount of memory used by an algorithm grows as the input size increases.

**Example:** An algorithm that creates a second array containing one item for every input element uses `O(n)` additional space.

## References

1. NIST. *Dictionary of Algorithms and Data Structures*. https://xlinux.nist.gov/dads/
2. OpenDSA. *Data Structures and Algorithms*. https://opendsa.org/
3. Cormen, T. H., Leiserson, C. E., Rivest, R. L., and Stein, C. *Introduction to Algorithms* (4th ed.). MIT Press, 2022.
