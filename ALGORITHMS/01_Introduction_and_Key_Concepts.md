
# Algorithms

## 1.1 What Is an Algorithm?

An **algorithm** is a sequence of clear, ordered instructions used to solve a problem or complete a task. An algorithm explains what steps should be followed, in what order, and when the task is finished.

Algorithms are not only used in computer science. We use them in everyday life, often without realizing it.

For example, imagine making a cup of tea:

1. Fill a kettle with water.
2. Heat the water until it boils.
3. Put a tea bag into a cup.
4. Pour the hot water into the cup.
5. Wait a few minutes.
6. Remove the tea bag.

These steps form an algorithm because they describe how to complete a task in a logical order.

In computer science, algorithms are used to solve problems such as finding information, organizing data, calculating results, and recommending videos or products. Computers can perform these tasks quickly, but they need instructions that are clear enough to follow.

A useful algorithm should have several important characteristics:

- **Clear instructions:** Each step should be understandable and specific.
- **Correctness:** The algorithm should produce the expected result when used under the right conditions.
- **A definite ending:** It should finish after a limited number of steps rather than continue forever.
- **An appropriate order:** Steps should be arranged so that the task can be completed correctly.

### Example: Finding a Student's Name

Imagine that a teacher has a list of student names and needs to find one particular student.

A simple algorithm could be:

1. Start with the first name on the list.
2. Compare it with the name you are looking for.
3. If the names match, stop and report that the student has been found.
4. If they do not match, move to the next name.
5. Repeat until the name is found or the list ends.
6. If the list ends without a match, report that the name is not on the list.

This is an example of a **searching algorithm**. It provides a systematic way to find information instead of checking names randomly.

The same idea can be applied to finding a book in a library, looking for a product in an online store, or locating a file on a computer.

## 1.2 Why Are Algorithms Important?

Algorithms are important because they help us solve problems in a systematic and efficient way. They allow computers to process information, make calculations, and complete tasks consistently.

For example, when you search for a video, a map location, or a product online, algorithms help the application process your request and find relevant information.

However, not all algorithms solve a problem equally well. Some require more steps or more time than others. Choosing an appropriate algorithm can make a significant difference, especially when working with large amounts of data.

### Example: Finding a Name in a List of 1,000 Students

Imagine that you need to find one student's name in a list containing 1,000 names.

There are different ways to approach this problem.

#### Method 1: Check Every Name

You begin with the first name and check each name one by one until you find the student.

This method is simple and works even if the names are not arranged in any particular order. However, if the student is near the end of the list, you may need to check almost all 1,000 names.

#### Method 2: Repeatedly Divide the List in Half

Suppose the names are arranged in alphabetical order. You can use a different approach:

1. Check the name in the middle of the list.
2. If the target name comes alphabetically before it, continue searching in the first half.
3. If the target name comes after it, continue searching in the second half.
4. Repeat the process with the remaining half until the name is found or no names remain.

This method is called **binary search**. Instead of checking every name, it eliminates approximately half of the remaining possibilities at each step.

For a list of 1,000 names, a binary search needs at most about 10 comparisons under the usual conditions, while checking names one by one could require up to 1,000 comparisons.

The important difference is that binary search requires the list to be sorted. If the names are not in order, this method cannot be applied directly.

### What Makes an Algorithm Efficient?

An algorithm's efficiency describes how many resources it needs to solve a problem. Two important resources are:

- **Time:** How many steps or how much processing time does the algorithm require?
- **Memory:** How much computer storage space does it need while working?

An algorithm that works well for a list of 10 items might be inefficient for a list of one million items. Therefore, computer scientists study how algorithms behave as the amount of data increases.

**Key idea:** A good algorithm should solve the problem correctly and use resources appropriately. The fastest method is not always necessary for a small task, but efficiency becomes increasingly important when dealing with large amounts of data.

## 1.3 Searching Algorithms

A **searching algorithm** is a method used to find a particular item in a collection of data.

For example, searching algorithms can help you find a name in a student database, a product in an online shop, or a number in a list.

Two basic searching algorithms are linear search and binary search.

### 1.3.1 Linear Search

**Linear search** finds an item by checking elements one by one, starting from the beginning of the collection.

It is one of the simplest searching algorithms and does not require the data to be sorted.

#### Example

Suppose we have the following list of numbers:

`[4, 9, 7, 2, 6]`

We want to find the number `7`.

We follow these steps:

1. Check the first number: `4`. It is not `7`.
2. Check the second number: `9`. It is not `7`.
3. Check the third number: `7`. We have found the target.
4. Stop searching.

The algorithm has found the number after checking three elements.

If we were looking for `2`, we would need to check four elements. If we were looking for a number that was not in the list, we would need to check all five elements before concluding that it was missing.

#### Linear Search: Step-by-Step

| Step | Number Checked | Result |
|---|---:|---|
| 1 | 4 | Not found |
| 2 | 9 | Not found |
| 3 | 7 | Found! |

#### Advantages and Disadvantages

**Advantages:**

- Easy to understand and implement.
- Works with sorted and unsorted data.
- Suitable for small lists.

**Disadvantages:**

- Can require many comparisons when the list is large.
- Must check every element if the target is at the end or is not present.

Linear search is useful when a collection is small or when the data has not been sorted.

### 1.3.2 Binary Search

**Binary search** is a searching algorithm that repeatedly divides a sorted list into smaller parts to find a target value.

Unlike linear search, binary search requires the elements to be arranged in order. For numbers, this usually means smallest to largest or largest to smallest.

Instead of checking every element, binary search examines the middle element and uses the result to decide which half may contain the target.

#### Example

Consider this sorted list:

`[2, 4, 6, 8, 10, 12, 14, 16]`

We want to find the number `14`.

**Step 1: Check the Middle**

The middle of the list is around `8`. For an even-sized list, either of the two central elements can be selected.

Since `14` is greater than `8`, it cannot be in the lower half. We continue with the upper half:

`[10, 12, 14, 16]`

**Step 2: Check the Middle of the Remaining Part**

We check `12`.

Since `14` is greater than `12`, we continue with the part to its right:

`[14, 16]`

**Step 3: Check the Next Middle Element**

We check `14`.

The target matches, so the search stops.

The algorithm has found the target without checking every number in the original list.

#### Binary Search: Step-by-Step

| Step | Value Checked | Decision |
|---|---:|---|
| 1 | 8 | Search the upper half |
| 2 | 12 | Search the upper half again |
| 3 | 14 | Target found |

#### Advantages and Disadvantages

**Advantages:**

- Very efficient for large, sorted collections.
- Eliminates approximately half of the remaining search area at each step.

**Disadvantages:**

- Requires sorted data.
- Is more complicated to implement than linear search.
- If the data is not sorted, sorting it first may require additional time and resources.

### 1.3.3 Linear Search vs. Binary Search

| Feature | Linear Search | Binary Search |
|---|---|---|
| How it works | Checks elements one by one | Repeatedly divides the search area in half |
| Requires sorted data? | No | Yes |
| Best suited for | Small or unsorted collections | Large, sorted collections |
| Worst-case comparisons for `n` items | Up to `n` | About `log₂(n) + 1` |
| Main advantage | Simple and flexible | Efficient for large, sorted data |

The expression `log₂(n)` describes how many times a collection can be divided in half before reaching a very small size. You do not need to understand logarithms in detail to understand the main idea: repeatedly halving a large collection can reduce the number of comparisons dramatically.

**Remember:** Linear search checks items one by one. Binary search uses the order of the data to eliminate large parts of the list.

## 1.4 Sorting Algorithms

A **sorting algorithm** arranges data in a particular order. The data may be arranged from smallest to largest, largest to smallest, or alphabetically.

Sorting is useful because organized data is often easier to understand and search.

For example, sorting can help you:

- Arrange student grades from highest to lowest.
- Organize products by price.
- Display names alphabetically.
- Arrange dates from earliest to latest.
- Prepare data for certain searching algorithms, such as binary search.

Different sorting algorithms use different methods to arrange the same data.

### 1.4.1 Insertion Sort

**Insertion sort** is a sorting algorithm that builds a sorted list one element at a time.

It works in a similar way to arranging playing cards in your hand. You take one card at a time and insert it into the correct position among the cards you have already arranged.

Insertion sort begins by treating the first element as sorted. It then takes each remaining element and places it in the correct position within the sorted part.

#### Example

Suppose we want to sort this list in ascending order:

`[5, 2, 8, 1]`

**Step 1: Start with the First Element**

We begin with `5`. Since there is only one element, it is already sorted.

`[5 | 2, 8, 1]`

The vertical line separates the sorted part from the unsorted part.

**Step 2: Insert 2 into the Correct Position**

The next element is `2`.

Since `2` is smaller than `5`, we move `5` to the right and insert `2` before it.

`[2, 5 | 8, 1]`

Now the sorted part is `[2, 5]`.

**Step 3: Insert 8 into the Correct Position**

The next element is `8`.

Since `8` is greater than `5`, it already belongs at the end of the sorted part.

`[2, 5, 8 | 1]`

**Step 4: Insert 1 into the Correct Position**

The final element is `1`.

It is smaller than `8`, `5`, and `2`, so these elements move one position to the right. We insert `1` at the beginning.

`[1, 2, 5, 8]`

The list is now sorted in ascending order.

#### Insertion Sort: Summary

| Step | List |
|---|---|
| Original list | `[5, 2, 8, 1]` |
| Insert 2 | `[2, 5, 8, 1]` |
| Insert 8 | `[2, 5, 8, 1]` |
| Insert 1 | `[1, 2, 5, 8]` |

The algorithm works by expanding the sorted part until every element has been placed in its correct position.

#### Advantages and Disadvantages

**Advantages:**

- Easy to understand.
- Works well with small lists.
- Can be efficient when the data is already almost sorted.
- Does not require a separate collection to store the sorted list in its basic form.

**Disadvantages:**

- Can be slow for large, randomly ordered lists.
- May need to move many elements to insert a single value.

Insertion sort is a useful starting point for learning how sorting algorithms work. More advanced algorithms can be more efficient when working with very large collections.

### 1.4.2 Why Are There Different Sorting Algorithms?

There is no single sorting algorithm that is best for every situation.

For a small list, insertion sort may be a good choice because it is simple and has little overhead. For a very large collection, other algorithms, such as merge sort, may be more efficient.

The choice depends on factors such as:

- The amount of data.
- Whether the data is already partly sorted.
- The time available for processing.
- The amount of memory available.

Understanding different algorithms helps programmers choose an appropriate solution for a particular problem.

## Sources

1. Khan Academy, [Algorithms](https://en.khanacademy.org/computing/computer-science/algorithms).
2. MIT OpenCourseWare, [Introduction to Algorithms — Lecture Notes](https://ocw.mit.edu/courses/6-006-introduction-to-algorithms-fall-2011/pages/lecture-notes/).
3. Khan Academy, [Binary Search](https://www.khanacademy.org/computing/computer-science/algorithms/binarysearch/a/binary-search).
4. Khan Academy, [Insertion Sort](https://en.khanacademy.org/computing/computer-science/algorithms/insertion-sort/a/insertion-sort).
