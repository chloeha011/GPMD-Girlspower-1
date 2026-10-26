# Algorithms – Learning Goals, Explanations and Guidance

## 1. Who This Section Is For

This material is written for people who are completely new to computer science and artificial intelligence.  
The explanations stay simple and clear. The goal is not to turn beginners into experts. The goal is to help them understand the basic ideas and feel less scared of the topic.

---

## 2. What Are Learning Goals?

Learning goals are the main things we want people to understand or be able to do after they finish the materials on Algorithms.  
They tell us what success looks like.

---

## 3. Main Learning Goals for Algorithms

### Goal 1: Understand what an algorithm is

An algorithm is a clear list of steps used to solve a problem.

**Example:**  
A recipe for cooking is a kind of algorithm. It tells you exactly what to do, in what order, to reach a result.

**Learning outcomes:**
- Explain what an algorithm is in their own words.
- Give one simple everyday example of an algorithm.
- Understand that different algorithms can take different amounts of time or use different amounts of memory when the problem gets bigger.
- Recognise that efficiency becomes more important as the size of the problem grows (without needing formal mathematics yet).

---

### Goal 2: Follow and create simple step-by-step instructions

**Learning outcomes:**
- Follow a written list of steps and produce the correct result.
- Break a simple problem into smaller, clear steps.
- Describe the steps of a basic algorithm out loud or in writing.
- Feel comfortable reading a short sequence of instructions and understanding what it does.

---

### Goal 3: Know a few classic simple algorithms

**Learning outcomes:**
- Describe linear search (checking items one by one from the beginning).
- Describe how to find the maximum or minimum value in a list of numbers.
- Understand the basic idea of a simple sorting method (building a sorted section one item at a time).
- Recognise these algorithms when they appear in simple examples.

---

### Goal 4: Understand the basic idea of efficiency

**Learning outcomes:**
- Understand that some methods take more steps than others.
- See that the number of steps often grows when the amount of data grows.
- Understand why we care about efficiency, even if we do not yet use formal mathematical notation.
- Compare two simple ways of solving the same problem and notice which one does more work.

---

### Goal 5: Move from only reading to actually trying

**Learning outcomes:**
- Run or carefully follow simple examples.
- Change small parts of an example (for example the list of numbers) and observe what happens.
- Feel that they can experiment without being completely lost.
- Gain confidence to continue learning.

---

### Goal 6: Feel more confident about the topic

Many beginners feel that algorithms are too abstract or too difficult.  

**Learning outcomes:**
- Feel that they understand the basic ideas.
- Feel that they can continue learning without being completely lost.
- Be able to explain the main ideas to another beginner in simple language.

---

## 4. Detailed Explanations

### 4.1 What is an algorithm?

An algorithm is a clear, ordered list of steps that solves a problem or completes a task.  
It must be precise enough that another person (or a computer) can follow it without guessing.

**Everyday examples:**

- A cooking recipe  
- Directions to a friend’s house  
- The way you sort a deck of cards by hand  
- The steps to log into an email account  

**Key characteristics of a good algorithm:**
- Clear inputs (what information is needed at the start)
- Clear outputs (what result is produced)
- Correctness (it gives the right answer)
- Finiteness (it finishes after a limited number of steps)
- Clarity (another person can understand the steps)

---

### 4.2 Linear Search

Linear search is the simplest way to look for a value in a list.

**How it works:**
1. Start at the first item in the list.
2. Compare it with the value you are looking for.
3. If it matches, stop — you found it.
4. If it does not match, move to the next item.
5. Repeat until you find the value or reach the end of the list.

**Important observations:**
- Best case: the item is the first one → only one step is needed.
- Worst case: the item is the last one or is not in the list → every item must be checked.
- Linear search always works, even if the list is not sorted.

This algorithm is easy to understand and is a good starting point for beginners.

---

### 4.3 Finding the Maximum or Minimum

**Algorithm to find the maximum value:**
1. If the list is empty, there is no maximum.
2. Assume the first number is the largest so far.
3. Look at each of the remaining numbers one by one.
4. Whenever you see a number that is bigger than the current maximum, update the current maximum.
5. When you have checked every number, the current maximum is the answer.

The same idea works for the minimum — you simply keep the smallest number instead of the largest.

This is a clear example of algorithmic thinking: breaking a problem into small, precise steps.

---

### 4.4 Simple Sorting – The Insertion Sort Idea

Sorting means arranging items in order (usually from smallest to largest).

**Everyday analogy:**  
Imagine you are sorting playing cards in your hand.  
The cards already in your hand are in order. You take the next card and insert it into the correct place among the cards you already hold.

**In a list of numbers the same idea is used:**
- Start with the first item (a list of one item is already sorted).
- Take the next item and insert it into the correct position in the already-sorted part.
- Repeat until every item has been inserted.

Insertion sort is not the fastest sorting method for very large lists, but it is excellent for learning because the idea is easy to follow.

---

### 4.5 The Basic Idea of Efficiency

Different algorithms can solve the same problem with very different numbers of steps.

When the amount of data is small, the difference may not matter much.  
When the amount of data becomes large, the difference can become enormous.

**Intuitive categories (no formal mathematics required yet):**

- **Constant work** – the number of steps stays roughly the same even if the data grows.
- **Linear growth** – the number of steps grows in proportion to the size of the data (example: linear search).
- **Quadratic growth** – the number of steps grows much faster (size × size).

For beginners it is enough to understand that:
- Some methods take more steps than others.
- Efficiency becomes more important as problems grow.
- Choosing a better method can save a lot of time when the data becomes large.

---

## 5. How Algorithms Connect to the Rest of the Project

- Algorithms are the step-by-step methods we use to solve problems.
- Data structures are the ways we organise information so that algorithms can work efficiently.
- Connectionist AI (neural networks) still relies on algorithms and data structures underneath.

Understanding basic algorithms makes the other two topics easier and less intimidating.

---

## 6. Possible Challenges for Beginners

- The idea of “efficiency” can feel abstract at first.
- It is easy to focus only on theory and forget to follow examples step by step.
- Some learners feel that algorithms are only for advanced students.

**How we address these challenges:**
- We use everyday analogies.
- We keep the language simple.
- We focus on understanding rather than formal mathematics.
- We encourage learners to follow steps by hand and then try small changes.

---

## 7. What Success Looks Like

If a person who knew nothing about the topic can:
- Explain what an algorithm is in their own words
- Give a simple everyday example
- Describe linear search and finding a maximum
- Understand why the number of steps matters
- Feel less afraid of the subject

…then the learning goals for Algorithms have been reached.

---

## 8. Final Note

These learning goals and explanations will guide everything created for the Algorithms part of the project — the explanations, the examples, and the simple exercises.  

Keeping them simple and clear is the most important part, because the audience is starting from zero.
