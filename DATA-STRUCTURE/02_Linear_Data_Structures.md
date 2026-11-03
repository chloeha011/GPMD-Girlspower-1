# Linear Data Structures

## 1. Definition

A linear data structure organizes data elements in a single logical sequence. Each element has a position in that sequence, so elements can be processed one after another.

Examples include arrays, linked lists, stacks, and queues. Unlike non-linear structures such as trees and graphs, which can branch into multiple paths, linear structures follow one main sequence.

A linear data structure also defines how data is accessed, inserted, removed, and processed. The performance of these operations depends on the structure's design and implementation.

## 2. How Linear Data Structures Work

Linear data structures arrange elements in a logical order. Consider this sequence:

`A → B → C → D`

- A is the first element.
- B follows A, and C follows B.
- D is the last element.

A program can traverse the sequence by visiting its elements in order. However, the way it reaches each element depends on the structure: arrays support access by index, while linked lists are usually traversed from node to node.

### General Process

1. Store data according to the structure's rules.
2. Access elements by index, position, or sequence.
3. Insert new elements at permitted positions.
4. Remove elements while maintaining the required order.
5. Traverse the structure when processing its contents.

### Memory Organization

Linear data structures can use different memory arrangements:

- **Contiguous memory:** Elements are stored next to one another in memory. Arrays commonly use this arrangement.
- **Linked memory:** Elements are stored in separate nodes connected by references or pointers. Linked lists use this arrangement.

These arrangements affect how quickly elements can be accessed and how efficiently elements can be inserted or removed.

## 3. Characteristics of Linear Data Structures

- **Sequential organization:** Elements follow one logical order.
- **Ordered traversal:** Elements can be visited one after another.
- **Position-based operations:** Elements can be accessed, inserted, or removed according to the rules of the structure.
- **Order preservation:** Operations generally maintain the sequence of the remaining elements.
- **Different performance:** Some structures are designed for fast access, while others make insertion or removal at particular positions more convenient.

## 4. Common Linear Data Structures and Their Implementations

Linear data structures should not be classified simply as “static” or “dynamic.” These terms describe how an implementation manages its size, not separate types of linear data structures. For example, arrays may have a fixed capacity or be implemented as dynamic arrays that can resize.

### 4.1 Array

An array stores elements in indexed positions, usually in consecutive memory locations. This allows a program to access an element directly using its index.

Example:

`Index:  0   1   2   3`

`Value: 10  20  30  40`

**How it works**

- Each element has an index, commonly starting at 0.
- The index is used to locate an element directly.
- Accessing an element by index typically takes O(1) time.

**Advantages**

- Fast access by index.
- Simple to use and traverse.
- Contiguous storage can provide efficient memory access.

**Limitations**

- Inserting or removing an element near the beginning or middle usually requires shifting other elements.
- A fixed-size array cannot change its capacity after creation.
- A dynamic array can grow, but resizing may require allocating new memory and copying elements.

**Common applications**

- Storing student grades.
- Representing image pixels.
- Maintaining lists of values for processing.

### 4.2 Linked List

A linked list consists of nodes connected through references or pointers. Each node stores data and a link to another node. In a singly linked list, each node points to the next node.

Example:

`10 → 20 → 30 → 40 → NULL`

**How it works**

- Each node stores a value and a reference to the next node.
- The list begins at a reference called the head.
- To reach a particular element, the program usually follows the links from the head.

**Advantages**

- Can grow or shrink as nodes are added or removed.
- Insertion or deletion can be efficient when the relevant node and links are already known.
- Does not require all nodes to be stored next to one another in memory.

**Limitations**

- Accessing an element by position requires traversal, so it typically takes O(n) time.
- Each node requires extra memory for its reference.
- Managing links makes implementation more complex than a basic array.

**Common applications**

- Implementing stacks and queues.
- Managing sequences of items that change frequently.
- Representing certain navigation or memory-management structures.

## 5. Specialized Linear Data Structures

Some linear data structures follow specific rules for inserting and removing elements.

### 5.1 Stack (LIFO)

A stack follows the **Last In, First Out (LIFO)** principle. The last element added is the first one removed.

Imagine a stack of books: the book placed on top most recently is the first one you can take off.

Example operations:

| Operation | Result |
| --- | --- |
| Push(10) | 10 is added |
| Push(20) | 20 is placed above 10 |
| Push(30) | 30 is placed above 20 |
| Pop() | Removes 30 |
| Peek() | Shows 20 without removing it |

**How it works**

All standard stack operations take place at the top.

- **Push:** Adds an element to the top.
- **Pop:** Removes the top element.
- **Peek:** Returns the top element without removing it.

**Applications**

- Undo operations in software.
- Managing function calls.
- Evaluating expressions.

### 5.2 Queue (FIFO)

A queue follows the **First In, First Out (FIFO)** principle. The first element added is the first one removed.

Imagine people waiting in a line: the person who arrives first is served first.

Example:

`Front → A → B → C ← Rear`

Operations:

- **Enqueue(D):** Adds D at the rear.
- **Dequeue():** Removes A from the front.

After removing A and adding D:

`Front → B → C → D ← Rear`

**How it works**

- New elements enter at the rear.
- Elements are removed from the front.
- A suitable implementation, such as a circular array or linked list, avoids shifting all remaining elements after each removal.

**Applications**

- Print jobs.
- Task scheduling.
- Customer service systems.
- Network packet processing.

## 6. Comparison of Linear Data Structures

The table below shows typical time complexities. Actual performance can vary depending on the implementation and the operation being performed.

| Structure | Access | Insertion | Deletion |
| --- | --- | --- | --- |
| Array | O(1) by index | O(n) at the beginning or middle; typically O(1) amortized when appending to a dynamic array | O(n) at the beginning or middle |
| Linked List | O(n) by position | O(1) when the insertion point and required link are already known | O(1) when the target node and required link are already known |
| Stack | Top element: O(1) | Push: typically O(1) | Pop: typically O(1) |
| Queue | Front element: O(1) | Enqueue: typically O(1) | Dequeue: typically O(1) |

**Notes:**

- **O(1)** means the operation takes constant time, regardless of the number of elements.
- **O(n)** means the time required grows in proportion to the number of elements.
- Appending to a dynamic array is typically O(1) amortized: most appends are constant time, but occasional resizing takes longer.
- Stack and queue operations are typically O(1) when implemented appropriately. A dynamic implementation may occasionally need to resize.
- Linked-list insertion and deletion are O(1) only when the relevant node or position and the links needed for the operation are already available. Finding the position first may take O(n).

## 7. Worked Example

Suppose a customer service system processes requests in the order they arrive.

Requests arrive in this order:

1. Customer A
2. Customer B
3. Customer C

A queue stores them as:

`Front → A → B → C ← Rear`

The service process becomes:

| Step | Queue |
| --- | --- |
| Enqueue A | A |
| Enqueue B | A → B |
| Enqueue C | A → B → C |
| Dequeue | B → C |
| Enqueue D | B → C → D |

Customer A is served first because a queue follows the FIFO principle.

## 8. Practice Activity

A stack performs these operations:

1. Push(A)
2. Push(B)
3. Push(C)
4. Pop()
5. Push(D)
6. Peek()

### Questions

1. Which element is removed?
2. Which element appears at the top after all operations?
3. Why does a stack behave differently from a queue?

### Expected Answers

- Pop() removes C.
- After D is pushed, D is at the top.
- A stack follows LIFO, while a queue follows FIFO. Therefore, a stack removes the most recently added element first, whereas a queue removes the earliest added element first.

## 9. Why Linear Data Structures Matter

Linear data structures provide practical ways to organize and process data in a sequence. They are used in software applications, operating systems, databases, and many other areas of computing. Understanding arrays, linked lists, stacks, and queues helps programmers choose a suitable structure based on the operations a program needs to perform and the trade-offs in access speed, insertion, deletion, and memory use.

## References

1. OpenDSA. *Data Structures and Algorithms*. [https://opendsa-server.cs.vt.edu/](https://opendsa-server.cs.vt.edu/)
2. Python Software Foundation. *Data Structures*. [https://docs.python.org/3/tutorial/datastructures.html](https://docs.python.org/3/tutorial/datastructures.html)
3. Cormen, T. H., et al. *Introduction to Algorithms*. MIT Press.