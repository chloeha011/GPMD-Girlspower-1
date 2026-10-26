# Data Structures: Examples and Learner Activities

## 1. Examples of Data Structures

### Example 1: Array

**Scenario:** A teacher stores students' examination scores.

```python
scores = [85, 90, 78, 92, 88]

print(scores[0])  # Output: 85
print(scores[2])  # Output: 78
```

**Explanation:** An array or list stores multiple values in an ordered collection. Each element can be accessed using its index.

### Example 2: Stack

**Scenario:** A text editor uses an undo mechanism to reverse recent actions.

```python
stack = []

stack.append("Write")
stack.append("Delete")
stack.append("Edit")

print(stack.pop())  # Output: Edit
```

**Explanation:** A stack follows the LIFO principle (Last In, First Out). The last element added is the first one removed.

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

**Explanation:** A queue follows the FIFO principle (First In, First Out). The first element added is the first one removed.

### Example 4: Linked List

**Scenario:** Each element points to the next element in a sequence.

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

while current:
    print(current.data)
    current = current.next
```

**Output:**
```text
10
20
30
```

**Explanation:** A linked list consists of nodes containing data and references to other nodes.

### Example 5: Tree

**Scenario:** A university organizes its departments under different faculties.

```text
          University
          /        \
    Faculty A     Faculty B
      /   \         /   \
    CS   Maths   Art   Business
```

**Explanation:** A tree organizes data hierarchically through parent-child relationships.

### Example 6: Graph

**Scenario:** A navigation application represents cities connected by roads.

```text
       City A
       /     \
   City B — City C
       \     /
       City D
```

**Explanation:** A graph consists of vertices (nodes) connected by edges. It can represent roads, social networks, and other relationships.

---

## 2. Learner Activities

### Activity 1: Identify the Data Structure

**Task:** Match each situation with the most appropriate data structure.

1. Storing students' examination scores.
2. Reversing actions in a text editor.
3. Managing customers waiting in a queue.
4. Organizing files into folders and subfolders.
5. Representing connections between cities.

**Options:** Array/List, Stack, Queue, Tree, Graph.

**Challenge:** Explain why each data structure is suitable for its situation.

### Activity 2: Create an Array

**Task:** Write a Python program that stores five favorite movies or games in a list.

Requirements:
- Display the entire list.
- Print the first element.
- Add another item.
- Display the updated list.

**Challenge:** Remove one item and print the final list.

### Activity 3: Simulate a Stack

**Task:** Create a stack using a Python list.

Perform these operations:
1. Push the number `5`.
2. Push the number `10`.
3. Push the number `15`.
4. Remove one element.
5. Display the remaining elements.

**Questions:**
- Which element is removed first?
- What does LIFO mean?
- What happens when you remove an element from an empty stack?

### Activity 4: Manage a Queue

**Task:** Create a queue containing three student names.

Requirements:
1. Add three students.
2. Display the queue.
3. Remove the first student.
4. Add another student.
5. Display the updated queue.

**Questions:**
- Which student is served first?
- How does a queue differ from a stack?

### Activity 5: Build a Linked List

**Task:** Create a linked list containing the values `10`, `20`, and `30`.

Requirements:
- Create three nodes.
- Connect the nodes.
- Traverse the linked list.
- Print each node's value.

**Challenge:** Add a fourth node containing `40`.

### Activity 6: Draw a Tree

**Task:** Draw a tree representing a university's organizational structure.

Requirements:
- Create one root node representing the university.
- Add three faculties.
- Add two departments under each faculty.

**Questions:**
- Which node is the root?
- What are the child nodes?
- How are the nodes connected?

### Activity 7: Design a Graph

**Task:** Create a graph representing five cities connected by roads.

Requirements:
- Represent each city as a node.
- Connect cities using edges.
- Identify two possible routes between cities if the graph allows them.

**Challenge:** Explain how a navigation application could use this graph to find a route.

---

## 3. Mini Programming Challenge

### Student Waiting List

**Task:** Write a Python program that manages students waiting for assistance.

Requirements:
1. Create an empty queue.
2. Add three students.
3. Display the waiting list.
4. Process the first student.
5. Display the remaining students.

**Expected output:**

```text
Waiting list: ['Ali', 'Malika', 'John']
Student served: Ali
Remaining students: ['Malika', 'John']
```

**Extension:** Allow the user to enter student names and choose whether to add a student or serve the next student.

---

## 4. Reflection Questions

After completing the activities, answer the following questions:

1. Which data structure was easiest to understand, and why?
2. What is the difference between a stack and a queue?
3. Which data structure would you use to represent a social network?
4. Why is it important to select an appropriate data structure?
5. How can data structures help solve real-world problems?
