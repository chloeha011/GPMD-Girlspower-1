# Algorithms: Introduction and Key Concepts

## 1.1 What Is an Algorithm?

An **algorithm** is a clear, ordered set of instructions for solving a problem or completing a task. It explains what steps to follow, the order in which to follow them, and when to stop.

Algorithms are used in computer science, but they are also part of everyday life. For example, making a cup of tea involves a sequence of steps:

1. Fill a kettle with water.
2. Heat the water until it boils.
3. Place a tea bag in a cup.
4. Pour the hot water into the cup.
5. Wait for three minutes.
6. Remove the tea bag.

These steps form a simple algorithm because they describe an organized process with a clear result. If a step is missing or performed in the wrong order, the result may be different from what was expected.

In computer science, algorithms tell computers how to complete tasks such as searching for information, sorting data, and calculating results. A computer can process information quickly, but it needs instructions to know what to do.

### Characteristics of a Good Algorithm

A good algorithm should have the following characteristics:

- **Clear instructions:** Each step should be specific and easy to understand.
- **Correctness:** It should produce the expected result when given valid input.
- **A definite ending:** It should finish after a finite number of steps.
- **A logical order:** The steps should be arranged in a sequence that allows the task to be completed.
- **Defined input and output:** It should make clear what information is needed and what result it should produce.

### Example: Finding a Student's Name

Imagine that a teacher needs to find a particular student in a list of names. A simple approach is to check each name in order:

1. Start with the first name.
2. Compare it with the name being searched for.
3. If the names match, report that the student has been found and stop.
4. If they do not match, move to the next name.
5. Continue until the name is found or the list ends.
6. If the list ends without a match, report that the name was not found.

This is called **linear search**. It checks items one at a time until it finds the target or reaches the end of the list. The example also shows how an everyday problem can be expressed as a sequence of instructions.

## 1.2 Why Are Algorithms Important?

Algorithms help us solve problems in a systematic and reliable way. Instead of relying on guesswork, we can follow a defined process and check whether it produces the expected result.

Algorithms are used in many familiar technologies:

- **Map applications** use algorithms to find possible routes between locations.
- **Online stores** use algorithms to organize products and process searches.
- **Video platforms** use algorithms to recommend content based on different signals, such as viewing activity.
- **Banking systems** use algorithms to process transactions and detect unusual activity.

Different algorithms can solve the same problem, but they may require different amounts of time or memory. This matters when a computer needs to process a large amount of information. Choosing an appropriate algorithm can make a task more efficient and help a system respond faster.

## 1.3 An Introduction to Searching Algorithms

A **searching algorithm** is a method for finding a particular item in a collection of data. Two common examples are:

- **Linear search:** Checks each item one by one. It works with both sorted and unsorted data.
- **Binary search:** Repeatedly divides the search range in half. It can be used when the data is sorted.

For example, if you are looking for a name in an unsorted list, linear search is a suitable option. If the list is already arranged alphabetically, binary search may find the name with fewer comparisons, especially in a large list.

The detailed steps, examples, and comparison of these methods are covered in the next section.

## 1.4 An Introduction to Sorting Algorithms

A **sorting algorithm** arranges data in a chosen order, such as from smallest to largest, highest to lowest, or alphabetically.

Sorting makes information easier to read, compare, and manage. For example, a teacher may arrange student scores from highest to lowest, while an online store may display products from lowest to highest price.

Different sorting algorithms use different methods to arrange data. Some compare nearby items and swap them when they are in the wrong order; others build a sorted section one item at a time. The most suitable method depends on factors such as the amount of data and how it is arranged initially.

The next section introduces examples of sorting algorithms and explains how they work.

## 1.5 Understanding Algorithm Efficiency

An algorithm should produce the correct result, but it should also use computer resources appropriately. Two important measures are:

- **Time complexity:** Describes how the number of operations an algorithm performs grows as the input size increases.
- **Space complexity:** Describes how the amount of memory an algorithm uses grows as the input size increases.

For example, checking a short list of names one by one may take very little time. Searching a list containing thousands or millions of names may require much more work.

Computer scientists use **Big O notation**, such as `O(n)` and `O(log n)`, to describe how an algorithm's resource requirements grow as the input becomes larger. At this stage, the main idea is that an algorithm's performance on a small example may not show how well it will perform with much larger data.

The next section explains time complexity, space complexity, and Big O notation in more detail.

## 1.6 A Simple Algorithm Design Activity

Think of a task you complete regularly, such as preparing a school bag, making a sandwich, or organizing books.

Write an algorithm for that task using clear, numbered steps. Then review your instructions:

1. Is every step clear enough for another person to follow?
2. Are the steps in the correct order?
3. Is it clear when the process is finished?
4. What information or materials are needed at the beginning?
5. What should the final result be?

This activity focuses on the basic idea of an algorithm: turning a task into a clear sequence of instructions.

## Key Takeaways

- An algorithm is a clear, ordered set of instructions for solving a problem.
- A good algorithm has clear steps, produces a correct result, follows a logical order, and eventually finishes.
- Algorithms are used in everyday technology, including maps, online stores, and video platforms.
- Searching algorithms find information, while sorting algorithms arrange data in a chosen order.
- Algorithm efficiency describes how resource requirements, such as time and memory, grow as the input size increases.
- The most suitable algorithm depends on the problem and the data being processed.

## References

1. Khan Academy, [Algorithms](https://www.khanacademy.org/computing/computer-science/algorithms).
2. MIT OpenCourseWare, [Introduction to Algorithms — Lecture Notes](https://ocw.mit.edu/courses/6-006-introduction-to-algorithms-fall-2011/pages/lecture-notes/).
3. Khan Academy, [Binary Search](https://www.khanacademy.org/computing/computer-science/algorithms/binarysearch/a/binary-search).
