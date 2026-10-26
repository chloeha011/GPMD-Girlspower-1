# Data Structures – Learning Goals, Explanations and Guidance

## 1. Who This Section Is For

This material is written for people who are completely new to computer science and artificial intelligence.  
The explanations stay simple and clear. The goal is not to turn beginners into experts. The goal is to help them understand the basic ideas and feel less scared of the topic.

## 2. What Are Learning Goals?

Learning goals are the main things we want people to understand or be able to do after they finish the materials on Data Structures.  
They tell us what success looks like.

## 3. Main Learning Goals for Data Structures

### Goal 1: Understand what a data structure is

A data structure is a way of organising and storing information in a computer so that it can be used efficiently.

**Example:**  
A shopping list is a simple data structure. A phone book (where you look up a name to find a number) is another kind of data structure.

**Learning outcomes:**
- Explain what a data structure is in their own words.
- Give one simple everyday example of a data structure.
- Understand that different structures make different operations easier or faster.
- Recognise that choosing the right structure becomes more important as the amount of data grows.

### Goal 2: Learn the most common data structures for beginners

**Learning outcomes:**
- Name and describe the following structures:
  - Lists (or arrays)
  - Dictionaries (or hash tables)
  - Stacks
  - Queues
  - Simple trees
- Explain in simple words what each structure is good for.
- Match a structure to a simple real-life or programming situation  
  (for example: “I need to look up a name quickly → use a dictionary”).

### Goal 3: Understand basic operations

**Learning outcomes:**
- Understand the meaning of common operations such as add, remove, search, and access.
- See that different structures make some of these operations fast and others slower.
- Follow simple examples of these operations step by step.

### Goal 4: See the connection between data structures and algorithms

**Learning outcomes:**
- Understand that algorithms need data structures to work on.
- Recognise that a good choice of data structure can make an algorithm much faster or simpler.
- See that neural networks and other AI systems also rely on data structures to store and process information.

### Goal 5: Move from only reading to actually trying

**Learning outcomes:**
- Follow simple examples of each structure.
- Change small parts of an example and observe what happens.
- Feel that they can experiment without being completely lost.
- Gain confidence to continue learning.

### Goal 6: Feel more confident about the topic

Many beginners feel that data structures are too technical or too abstract.

**Learning outcomes:**
- Feel that they understand the basic ideas.
- Feel that they can continue learning without being completely lost.
- Be able to explain the main ideas to another beginner in simple language.

## 4. Detailed Explanations

### 4.1 What is a data structure?

A data structure is a particular way of organising and storing information so that it can be used efficiently.

Different structures make different operations easy or hard. Choosing the right structure is an important part of solving problems with computers.

**Everyday examples:**
- A shopping list → items in order
- A phone book or dictionary → fast lookup by name
- A stack of plates → last one on top is the first one taken off
- A queue of people at a ticket counter → first person to join is the first to be served
- A family tree → hierarchical relationships

### 4.2 Lists (or Arrays)

A list (or array) stores items in a sequence, one after another.

**Main characteristics:**
- Items have a position (starting from 0 or 1).
- You can quickly access an item if you know its position.
- Adding or removing items in the middle can require shifting other items.

**Good for:**
- Keeping a collection of items in order
- Going through items one by one
- Situations where you often need the item in a specific position

### 4.3 Dictionaries (or Hash Tables)

A dictionary stores pairs of keys and values.  
You give a key (for example a name) and quickly get the associated value (for example a phone number).

**Main characteristics:**
- Very fast lookup by key
- Keys must be unique
- Order of items is usually not important

**Good for:**
- Looking up information by name, ID, or any unique identifier
- Counting how many times something appears
- Storing settings or properties

**Simple example situation:**  
“I need to look up a student’s grade by their name very quickly” → use a dictionary.

### 4.4 Stacks

A stack follows the rule **Last-In, First-Out** (LIFO).

**Everyday analogy:**  
A stack of plates. The last plate you put on top is the first one you take off.

**Main operations:**
- Push → add an item to the top
- Pop → remove the item from the top

**Good for:**
- Undo features
- Checking matching brackets in code
- Keeping track of nested function calls
- Browser back-button history

### 4.5 Queues

A queue follows the rule **First-In, First-Out** (FIFO).

**Everyday analogy:**  
A line of people at a ticket counter. The first person to join the line is the first person to be served.

**Main operations:**
- Enqueue → add an item to the end of the line
- Dequeue → remove the item from the front of the line

**Good for:**
- Processing tasks in the order they arrive
- Print queues
- Waiting lists
- Breadth-first exploration of data

### 4.6 Simple Trees

A tree is a hierarchical structure with a starting point (the root) and branches.

**Everyday analogy:**  
A family tree or the folder structure on a computer.

**Main characteristics:**
- One root
- Each item can have children
- Useful for representing hierarchical relationships

**Good for:**
- File systems
- Organisation charts
- Decision processes
- Efficient searching when the tree is kept ordered (binary search trees)

### 4.7 Choosing the right structure

The same information can often be stored in different structures.  
The best choice depends on what you need to do most often:

- Need fast lookup by name or ID? → Dictionary
- Need to process items in the order they arrived? → Queue
- Need to undo the last actions? → Stack
- Need items in a simple ordered sequence? → List
- Need hierarchical relationships? → Tree

Learning to make this choice is one of the most practical skills in the topic.

## 5. How Data Structures Connect to the Rest of the Project

- Algorithms need data structures to store and organise the information they work on.
- A good data structure can make an algorithm much faster or simpler.
- Connectionist AI (neural networks) still needs ordinary data structures to store training data, weights, and intermediate results.

Data structures are not separate from algorithms and AI — they support them.

## 6. Possible Challenges for Beginners

- The names of the structures (stack, queue, dictionary, tree) can feel unfamiliar at first.
- It is easy to memorise definitions without understanding when to use each structure.
- Some learners feel that data structures are only important for advanced programming.

**How we address these challenges:**
- We use strong everyday analogies.
- We focus on “what is this good for?” instead of only “how is it built?”.
- We keep the language simple and avoid unnecessary technical detail.
- We encourage learners to match structures to real situations.

## 7. What Success Looks Like

If a person who knew nothing about the topic can:
- Explain what a data structure is in their own words
- Name the main beginner structures (list, dictionary, stack, queue, simple tree)
- Say what each structure is good for with a simple example
- Choose a suitable structure for a simple situation
- Feel less afraid of the subject

…then the learning goals for Data Structures have been reached.

## 8. Final Note

These learning goals and explanations will guide everything created for the Data Structures part of the project — the explanations, the examples, and the simple exercises.  

Keeping them simple and clear is the most important part, because the audience is starting from zero.
