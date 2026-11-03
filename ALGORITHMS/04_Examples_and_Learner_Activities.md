# Algorithms: Examples and Learner Activities

## 1. Learning Objectives

After completing this section, learners should be able to:

- Follow the steps of simple algorithms.
- Apply linear search, binary search, and basic sorting methods.
- Explain how an algorithm reaches its result.
- Choose a suitable algorithm for a given problem.

## 2. Worked Examples

The following examples demonstrate how searching and sorting algorithms work step by step.

### Example 1: Linear Search

Suppose we want to find `8` in the list:

`[3, 6, 8, 2, 9]`

Linear search checks each item from left to right until it finds the target.

```text
[3] → [6] → [8] → [2] → [9]
 1     2     3
             ↑
          Found!
```

**Steps:**

1. Check `3`. It is not the target.
2. Check `6`. It is not the target.
3. Check `8`. The target is found, so the search stops.

The target is found at position 3 after checking three elements.

**Key point:** Linear search stops as soon as the target is found. It can also be used with unsorted data.

### Example 2: Binary Search

Suppose we want to find `12` in the sorted list:

`[2, 4, 6, 8, 10, 12, 14]`

Binary search repeatedly divides the search area in half.

**Steps:**

1. Check the middle value, `8`. Since `12` is greater than `8`, continue searching the right half.
2. The remaining values are `[10, 12, 14]`. Check the middle value, `12`.
3. The target is found, so the search stops.

**Key point:** Binary search reduces the number of possible values at each step. However, the data must be sorted before using this method.

### Example 3: Sorting with Selection Sort

Suppose we want to sort the following list from smallest to largest:

`[5, 3, 8, 2]`

Selection sort repeatedly finds the smallest value in the unsorted part of the list and places it in the correct position.

| Step | Action | List |
|---|---|---|
| Start | Original list | `[5, 3, 8, 2]` |
| 1 | Find `2` and swap it with `5` | `[2, 3, 8, 5]` |
| 2 | The smallest remaining value is `3`, already in place | `[2, 3, 8, 5]` |
| 3 | Find `5` and swap it with `8` | `[2, 3, 5, 8]` |

The final sorted list is:

`[2, 3, 5, 8]`

**Key point:** Selection sort places the smallest remaining value into its correct position during each pass.

## 3. Learner Activities

Complete the following activities before checking the suggested answers.

### Activity A — Linear Search

Find `7` in the list:

`[4, 1, 7, 3, 9]`

1. Which items do you check, in order?
2. At which position is the target found?
3. How many elements are checked?

### Activity B — Bubble Sort

Sort the following list in ascending order using bubble sort:

`[4, 2, 5, 1]`

1. Compare adjacent elements and swap them when they are in the wrong order.
2. Show the list after each swap in the first pass.
3. What does the list look like after the first pass?

### Activity C — Choosing an Algorithm

A school has 5,000 student IDs stored in sorted order. You need to find one particular ID.

1. Would you choose linear search or binary search?
2. Why is this method more suitable?
3. What condition must be met for this method to work?

### Activity D — Selection Sort

Sort the following list in ascending order using selection sort:

`[7, 3, 6, 2]`

1. Identify the smallest value in the unsorted part during each pass.
2. Show the list after each pass.
3. Write down the final sorted list.

### Activity E — Understanding Algorithm Efficiency

Consider two algorithms that search for an item in a collection:

- Algorithm A checks each element one by one.
- Algorithm B repeatedly divides the search area in half.

Answer the following questions:

1. Which algorithm is linear search?
2. Which algorithm is binary search?
3. Which algorithm is generally more efficient for a large, sorted collection? Explain briefly.

## 4. Answers and Explanations

**Activity A — Linear Search**

1. Check `4`, then `1`, and finally `7`.
2. The target is at position 3.
3. Three elements are checked.

Linear search stops when it finds the target, so it does not need to check the remaining elements.

**Activity B — Bubble Sort**

Original list: `[4, 2, 5, 1]`

First pass:

- Compare `4` and `2`. Swap them: `[2, 4, 5, 1]`
- Compare `4` and `5`. No swap is needed.
- Compare `5` and `1`. Swap them: `[2, 4, 1, 5]`

The list after the first pass is:

`[2, 4, 1, 5]`

After the remaining passes, the final sorted list is:

`[1, 2, 4, 5]`

**Activity C — Choosing an Algorithm**

1. Binary search.
2. It repeatedly halves the search area, reducing the number of comparisons needed.
3. The student IDs must be sorted.

Binary search is generally more efficient for large, sorted collections than checking every element one by one.

**Activity D — Selection Sort**

Original list: `[7, 3, 6, 2]`

- Pass 1: Select `2` and swap it with `7`: `[2, 3, 6, 7]`
- Pass 2: Select `3`. It is already in the correct position: `[2, 3, 6, 7]`
- Pass 3: Select `6`. It is already in the correct position: `[2, 3, 6, 7]`

Final sorted list:

`[2, 3, 6, 7]`

**Activity E — Understanding Algorithm Efficiency**

1. Algorithm A is linear search.
2. Algorithm B is binary search.
3. Binary search is generally more efficient because it eliminates approximately half of the remaining search area at each step.

## 5. Key Takeaways

- Linear search checks elements one by one until the target is found or the collection ends.
- Binary search repeatedly halves the search area and requires sorted data.
- Bubble sort compares adjacent elements and swaps them when necessary.
- Selection sort repeatedly finds the smallest remaining element and places it in the correct position.
- Different algorithms can solve the same problem but may require different amounts of time and resources.
- Choosing an appropriate algorithm depends on the problem, the data, and the required efficiency.

## 6. Resources and References

1. **Khan Academy — Algorithms**  
   https://www.khanacademy.org/computing/computer-science/algorithms  
   Introductory materials on algorithms, searching, sorting, and efficiency.

2. **Khan Academy — Sorting Algorithms**  
   https://www.khanacademy.org/computing/computer-science/algorithms/sorting-algorithms  
   Further reading on sorting methods and how they arrange data.

3. **MIT OpenCourseWare — Introduction to Algorithms (6.006)**  
   https://ocw.mit.edu/courses/6-006-introduction-to-algorithms-spring-2020/  
   Lecture materials and exercises on algorithms and data structures.

These resources are provided for further learning and reference. Learners can use them to review the concepts and explore additional examples.
