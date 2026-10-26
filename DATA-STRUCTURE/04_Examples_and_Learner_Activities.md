# Data Structures: Examples and Learner Activities


## 1. Learning Objectives

After completing this section, learners should be able to explain how data structures organize information, compare common data structures, and choose a suitable structure for a simple problem.

## 2. Worked Example: Choosing a Data Structure

Imagine you are developing a student management system. Different tasks may require different ways to store information.

| Data Structure | Example | Why It Fits |
|---|---|---|
| Array | Students' exam scores | Stores items in order and allows access by index |
| Linked List | A sequence of tasks | Connects items through links between nodes |
| Stack | Undo actions in a text editor | The last action added is the first one removed |
| Queue | Students waiting for help | The first person waiting is usually served first |
| Tree | Folders on a computer | Represents hierarchical relationships |
| Graph | Connections between friends | Represents relationships between connected items |

No single data structure is best for every situation. The right choice depends on how the information will be stored, accessed, and changed.

## 3. Worked Example: Stack vs. Queue

A **stack** follows Last In, First Out (LIFO). A **queue** follows First In, First Out (FIFO).

**Stack example**

Imagine stacking books on a desk. You place Book A, then Book B, then Book C on top.

```text
Top -> Book C
       Book B
       Book A
```

If you remove one book, Book C comes out first because it was added last.

**Queue example**

Imagine three students waiting in line: A, B, and C.

```text
Front -> A -> B -> C <- Rear
```

Student A is served first because they joined the queue first.

## 4. Learner Activities

Try answering these questions before checking the answers.

### Activity A: Choose the Data Structure

Choose the most suitable data structure for each situation.

1. Keeping track of the browser's Back button history.
2. Managing customers waiting at a service counter.
3. Representing a family tree.
4. Representing routes between cities.

### Activity B: Understand the Operations

A stack is empty. The following operations are performed:

1. Push 10.
2. Push 20.
3. Push 30.
4. Pop one item.

What value is removed, and what values remain in the stack?

### Activity C: Apply Your Knowledge

A school wants to store student names in alphabetical order and frequently search for a particular student.

1. What information should the data structure store?
2. Why does keeping the names ordered help with searching?
3. Is the data structure choice affected by how often names are added or removed?

## 5. Answers and Explanations

**Activity A**

1. Stack — browser history commonly allows the most recently visited page to be returned from first.
2. Queue — customers are generally served in the order they arrive.
3. Tree — a family tree shows hierarchical relationships.
4. Graph — cities can be represented as vertices and routes as edges.

**Activity B**

The value **30** is removed. The stack then contains 20 on top of 10. This follows the LIFO principle: the last value added is the first value removed.

**Activity C**

1. The structure should store student names as data items.
2. Ordered names can make searching more efficient. For example, binary search can be used if the data is sorted and supports efficient access to the middle element.
3. Yes. If names are frequently added or removed, the cost of maintaining the order should also be considered.

## 6. Key Takeaways

- Data structures organize information so it can be used efficiently.
- Arrays, linked lists, stacks, queues, trees, and graphs serve different purposes.
- Stacks follow LIFO, while queues follow FIFO.
- Choosing a data structure depends on the operations a problem requires.
- A suitable structure can make a program easier to manage and more efficient.

## 7. Resources and References

1. **OpenDSA — Data Structures and Algorithms**  
   https://opendsa-server.cs.vt.edu/  
   A learning resource covering data structures, algorithms, and related concepts.

2. **VisuAlgo**  
   https://visualgo.net/en  
   Provides visual demonstrations of common data structures and algorithms.

3. **Programiz — Data Structures and Algorithms**  
   https://www.programiz.com/dsa  
   Offers beginner-friendly explanations and examples of common data structures.
