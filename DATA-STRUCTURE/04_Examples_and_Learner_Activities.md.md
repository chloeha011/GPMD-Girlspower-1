# Data Structures: Examples and Learner Activities

## 1. Practical Examples of Data Structures

The examples below show how common data structures organize information and support different operations. The Python examples use built-in features where possible.

### Example 1: Python List

**Scenario:** A teacher stores students' examination scores.

```python
scores = [85, 90, 78, 92, 88]

print(scores[0])  # Output: 85
print(scores[2])  # Output: 78

scores.append(95)
print(scores)
```

**Output:**
```text
85
78
[85, 90, 78, 92, 88, 95]
```

**Explanation:** A Python list stores multiple items in an ordered, changeable collection. Each item can be accessed by its index, starting at 0. A Python list is a dynamic sequence; it is not the same as a fixed-size array in every programming language.

### Example 2: Stack

**Scenario:** A text editor keeps track of recent actions so that the most recent action can be undone first.

```python
stack = []

stack.append("Write")
stack.append("Delete")
stack.append("Edit")

print(stack.pop())  # Output: Edit
print(stack)
```

**Output:**
```text
Edit
['Write', 'Delete']
```

**Explanation:** A stack follows the LIFO principle (Last In, First Out). The last item added is the first item removed. In Python, `append()` adds an item to the top of the stack, while `pop()` removes and returns the top item. Calling `pop()` on an empty list raises an error, so a program should check that the stack is not empty first.

### Example 3: Queue

**Scenario:** Students wait in line to receive assistance at a university office.

```python
from collections import deque

queue = deque(["Ali", "Malika", "John"])

queue.append("Sarah")
print(queue.popleft())  # Output: Ali
print(list(queue))
```

**Output:**
```text
Ali
['Malika', 'John', 'Sarah']
```

**Explanation:** A queue follows the FIFO principle (First In, First Out). The first item added is the first one removed. In Python, `deque` supports adding items to the back with `append()` and removing items from the front with `popleft()`. Removing an item from an empty deque raises an error.

### Example 4: Singly Linked List

**Scenario:** A sequence of connected nodes stores values, with each node referring to the next node.

```python
class Node:
    def __init__(self, data):
        self.data = data
        self.next = None

first = Node(10)
second = Node(20)
third = Node(30)

first.next = second
second.next = third

current = first
while current is not None:
    print(current.data)
    current = current.next
```

**Output:**
```text
10
20
30
```

**Explanation:** A singly linked list consists of nodes. Each node stores data and a reference to the next node. The first node is called the head. Traversal starts at the head and follows each reference until it reaches `None`, which marks the end of the list.

### Example 5: Tree

**Scenario:** A university organizes faculties and their departments in a hierarchy.

```text
             University
             /        \
       Faculty A     Faculty B
        /     \       /     \
      CS     Maths  Art   Business
```

**Explanation:** A tree organizes data through parent-child relationships. The university is the root, the faculties are its children, and the departments are lower-level nodes. In this example, each department has one parent, and the structure contains no cycles.

### Example 6: Graph

**Scenario:** A navigation application represents cities and the roads connecting them.

```text
A ----- B
|       |
|       |
C ----- D
```

The connections can be represented with an adjacency list:

```python
roads = {
    "A": ["B", "C"],
    "B": ["A", "D"],
    "C": ["A", "D"],
    "D": ["B", "C"]
}

print(roads["A"])  # Output: ['B', 'C']
```

**Explanation:** A graph consists of vertices (also called nodes) connected by edges. Here, each city is a vertex and each road is an edge. The example represents an undirected graph because each road can be travelled in both directions. A real navigation system may also store road distances, travel times, or one-way restrictions.

---

## 2. Learner Activities

Complete the activities to practise identifying, creating, and using different data structures.

### Activity 1: Identify the Data Structure

**Task:** Match each situation with the most suitable data structure.

1. Storing a collection of examination scores in order.
2. Reversing the most recent actions in a text editor.
3. Managing students waiting for assistance.
4. Organizing files into folders and subfolders.
5. Representing cities connected by roads.

**Options:** Python list, Stack, Queue, Tree, Graph.

**Challenge:** Explain which feature of each data structure makes it suitable. Could another structure also work? Explain your choice.

### Activity 2: Work with a Python List

**Task:** Write a Python program that stores five favourite movies or games in a list.

**Requirements:**
- Display the entire list.
- Print the first item.
- Add another item using `append()`.
- Display the updated list.

**Challenge:** Remove one item using `remove()` or `pop()` and display the final list. What is the difference between these two methods?

### Activity 3: Simulate a Stack

**Task:** Create a stack using a Python list.

Perform these operations:
1. Push the number `5`.
2. Push the number `10`.
3. Push the number `15`.
4. Pop one item.
5. Display the remaining stack.

**Questions:**
- Which item is removed, and why?
- What does LIFO mean?
- Why should a program check whether a stack is empty before calling `pop()`?

### Activity 4: Manage a Queue

**Task:** Use `collections.deque` to create a queue containing three student names.

**Requirements:**
1. Add three students to the queue.
2. Display the queue.
3. Remove the first student using `popleft()`.
4. Add another student.
5. Display the updated queue.

**Questions:**
- Which student is served first?
- How does a queue differ from a stack?
- Why is `deque` a suitable choice for implementing a queue in Python?

### Activity 5: Build a Linked List

**Task:** Create a singly linked list containing the values `10`, `20`, and `30`.

**Requirements:**
- Define a `Node` class with `data` and `next` attributes.
- Create three nodes and connect them.
- Start traversal at the head.
- Print each node's value until the end of the list.

**Challenge:** Add a fourth node containing `40` to the end of the list. Update the final node's `next` reference and display the list again.

### Activity 6: Draw a Tree

**Task:** Draw a tree representing a university's organizational structure.

**Requirements:**
- Create one root node representing the university.
- Add three faculties as child nodes.
- Add two departments under each faculty.

**Questions:**
- Which node is the root?
- Which nodes are children of the root?
- What is the relationship between a faculty and its departments?
- Why is a tree more suitable for this hierarchy than a simple list?

### Activity 7: Design a Graph

**Task:** Draw a graph representing five cities connected by roads.

**Requirements:**
- Represent each city as a vertex.
- Connect cities using edges.
- Label the edges if you want to show road distances.
- Identify two possible routes between a chosen pair of cities, if two routes exist.

**Questions:**
- Which cities are directly connected?
- Is your graph directed or undirected? Explain.
- How could a navigation application use the graph to compare possible routes?

---

## 3. Mini Design Challenge: Choose the Right Structure

**Scenario:** A university is developing a simple student-support application. The application needs to:

- Store a student's course names.
- Keep track of the most recent actions so they can be undone.
- Manage students waiting for help.
- Organize the university's faculties and departments.
- Represent connections between campus buildings.

**Task:** For each requirement, choose a suitable data structure and explain your reasoning.

**Extension:** Identify one limitation of each chosen structure. Suggest what additional information or feature the application might need to handle real-world situations.

---

## 4. Reflection Questions

After completing the activities, answer the following questions:

1. Which data structure was easiest to understand, and why?
2. What is the main difference between a stack and a queue?
3. How does a linked list differ from a Python list?
4. When would a tree be more suitable than a graph?
5. Why is it important to choose a data structure that fits the problem?
