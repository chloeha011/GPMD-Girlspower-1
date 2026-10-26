# Searching and Sorting Algorithms

## 2.1 Introduction

When working with data, we often need to find a particular item or arrange a collection into a more useful order. For example, a student may search for a name in a class list, while an online store may sort products by price.

In computer science, these tasks are handled by searching and sorting algorithms.

- **Searching algorithms** help us find a specific item in a collection of data.
- **Sorting algorithms** arrange data in a chosen order.

Different algorithms approach these tasks in different ways. Understanding how they work helps us choose a suitable method for a particular problem.

## 2.2 Searching Algorithms

### 2.2.1 Linear Search

**Linear search** finds an item by checking each element one at a time, starting from the beginning of the collection.

It does not require the data to be sorted, which makes it a simple and flexible method.

#### Example

Suppose we have the following list:

`[4, 9, 2, 7, 5]`

We want to find the number `7`.

1. Check `4`. It is not the target.
2. Check `9`. It is not the target.
3. Check `2`. It is not the target.
4. Check `7`. The target is found, so the search stops.

The algorithm checks four elements before finding the target.

| Step | Value Checked | Result |
|---|---:|---|
| 1 | 4 | Not found |
| 2 | 9 | Not found |
| 3 | 2 | Not found |
| 4 | 7 | Target found |

If the target is the first element, linear search finds it immediately. If it is near the end, the algorithm may need to check most of the list. If the target is not present, every element must be checked before the algorithm can conclude that the item is missing.

#### Advantages

- Easy to understand and implement.
- Works with both sorted and unsorted data.
- Useful for small collections or data that has not been organized.

#### Limitations

- May require many comparisons for large collections.
- In the worst case, it checks all `n` elements in a collection of size `n`.

### 2.2.2 Binary Search

**Binary search** finds a target by repeatedly dividing the search area in half.

Unlike linear search, binary search requires the data to be sorted. At each step, the algorithm checks a middle element and uses the result to decide which half may contain the target.

#### Example

Consider this sorted list:

`[2, 4, 6, 8, 10, 12, 14, 16]`

We want to find `14`.

**Step 1: Check the middle element**

Choose `8` as the middle element.

Since `14` is greater than `8`, the target must be in the upper half. We can ignore the lower half.

Remaining search area:

`[10, 12, 14, 16]`

**Step 2: Check the middle of the remaining area**

Choose `12`.

Since `14` is greater than `12`, continue with the values to its right.

Remaining search area:

`[14, 16]`

**Step 3: Check the next middle element**

Check `14`.

The value matches the target, so the search stops.

| Step | Value Checked | Decision |
|---|---:|---|
| 1 | 8 | Search the upper half |
| 2 | 12 | Search the upper half of the remaining area |
| 3 | 14 | Target found |

This example shows how binary search reduces the number of possible candidates at each step instead of checking every element.

#### Advantages

- Efficient for large collections of sorted data.
- Eliminates approximately half of the remaining search area at each step.

#### Limitations

- Requires sorted data.
- Is more complex to implement than linear search.
- Sorting an unsorted collection first may require additional work.

### 2.2.3 Linear Search vs. Binary Search

| Feature | Linear Search | Binary Search |
|---|---|---|
| Basic approach | Checks elements one by one | Repeatedly divides the search area in half |
| Requires sorted data? | No | Yes |
| Worst-case time complexity | `O(n)` | `O(log n)` |
| Main advantage | Simple and flexible | Efficient for large, sorted collections |
| Main limitation | Can require many comparisons | Cannot be applied directly to unsorted data |

Here, `n` represents the number of elements in the collection.

The notation `O(n)` means that the amount of work can grow roughly in proportion to the number of elements. The notation `O(log n)` describes a much slower rate of growth because the search area is repeatedly halved.

For example, linear search may check up to 1,000 elements in a list of 1,000 items. Binary search on a sorted list of the same size needs only about 10 comparisons in the usual implementation.

**Key idea:** Linear search is a good general-purpose method for small or unsorted collections. Binary search is often preferable when the data is already sorted and the collection is large.

## 2.3 Sorting Algorithms

A **sorting algorithm** arranges elements in a particular order. This section introduces two basic sorting algorithms: bubble sort and selection sort.

Both algorithms can arrange the same list into ascending order, but they use different methods to decide which elements should move.

### 2.3.1 Bubble Sort

**Bubble sort** repeatedly compares adjacent elements and swaps them when they are in the wrong order.

When sorting numbers from smallest to largest, a larger value moves toward the end of the list through a series of adjacent swaps. After each complete pass, the largest value in the unsorted section reaches its correct position.

#### Example

Suppose we want to sort this list in ascending order:

`[5, 3, 8, 2]`

**Pass 1**

1. Compare `5` and `3`. Swap them: `[3, 5, 8, 2]`
2. Compare `5` and `8`. They are already in the correct order.
3. Compare `8` and `2`. Swap them: `[3, 5, 2, 8]`

After the first pass, `8` is in its final position.

**Pass 2**

1. Compare `3` and `5`. No swap is needed.
2. Compare `5` and `2`. Swap them: `[3, 2, 5, 8]`

**Pass 3**

Compare `3` and `2`. Swap them:

`[2, 3, 5, 8]`

The list is now sorted.

#### Bubble Sort: Summary

| Stage | List |
|---|---|
| Original list | `[5, 3, 8, 2]` |
| After Pass 1 | `[3, 5, 2, 8]` |
| After Pass 2 | `[3, 2, 5, 8]` |
| After Pass 3 | `[2, 3, 5, 8]` |

#### Advantages

- Easy to understand and demonstrate.
- Shows how repeated comparisons and swaps can organize data.
- Can stop early if a complete pass makes no swaps, provided the implementation uses this optimization.

#### Limitations

- Performs many comparisons when the list is large.
- Has `O(n²)` average and worst-case time complexity in its standard form.

Bubble sort is useful for learning the basic idea of sorting, but it is generally not an efficient choice for large datasets.

### 2.3.2 Selection Sort

**Selection sort** works by repeatedly finding the smallest element in the unsorted part of a list and placing it at the beginning of that part.

Unlike bubble sort, which swaps adjacent elements, selection sort selects the smallest remaining value and moves it directly to its next correct position.

#### Example

Consider the list:

`[5, 3, 8, 2]`

We want to sort it in ascending order.

**Pass 1: Find the smallest element**

The smallest value is `2`. Swap it with the first element, `5`.

`[2, 3, 8, 5]`

The first element is now in its correct position.

**Pass 2: Find the smallest element in the remaining section**

Look at `[3, 8, 5]`.

The smallest value is `3`, which is already at the beginning of this section. No swap is needed.

`[2, 3, 8, 5]`

**Pass 3: Find the smallest element in the remaining section**

Look at `[8, 5]`.

The smallest value is `5`. Swap it with `8`.

`[2, 3, 5, 8]`

The list is now sorted.

#### Selection Sort: Summary

| Stage | List |
|---|---|
| Original list | `[5, 3, 8, 2]` |
| After Pass 1 | `[2, 3, 8, 5]` |
| After Pass 2 | `[2, 3, 8, 5]` |
| After Pass 3 | `[2, 3, 5, 8]` |

#### Advantages

- Straightforward to understand and implement.
- Performs at most `n - 1` swaps in its standard implementation.
- Can be useful when reducing the number of swaps is important.

#### Limitations

- Still performs many comparisons as the list grows.
- Has `O(n²)` average and worst-case time complexity.

Selection sort can reduce the number of swaps compared with some other simple sorting methods, but it is usually inefficient for large collections.

### 2.3.3 Bubble Sort vs. Selection Sort

Both algorithms sort data by repeatedly working through the unsorted part of a list. However, their main operations are different.

| Feature | Bubble Sort | Selection Sort |
|---|---|---|
| Main operation | Compares adjacent elements and swaps them when necessary | Finds the smallest remaining element and swaps it into position |
| What happens during a pass? | Larger values move toward the end | The smallest remaining value moves to the beginning of the unsorted section |
| Average time complexity | `O(n²)` | `O(n²)` |
| Worst-case time complexity | `O(n²)` | `O(n²)` |
| Main learning benefit | Demonstrates adjacent comparisons and repeated swaps | Demonstrates finding a minimum and placing it in the correct position |

Although both algorithms have quadratic time complexity in their standard forms, they behave differently while sorting. Following their steps side by side is a useful way to understand how different algorithms can solve the same problem.

## 2.4 Choosing an Appropriate Algorithm

There is no single algorithm that is best for every situation. The choice depends on the data and the task.

Consider these examples:

- **Finding a name in a short, unsorted list:** Linear search is simple and suitable.
- **Finding a value in a large, sorted list:** Binary search can reduce the number of comparisons.
- **Sorting a small list for learning purposes:** Bubble sort and selection sort are easy to demonstrate step by step.
- **Sorting a very large dataset:** More efficient sorting algorithms may be a better choice.

It is also important to consider whether the data is already sorted, how often the operation must be performed, and how much time and memory are available.

A useful algorithm is not necessarily the most complicated one. It is the one that meets the requirements of the problem while using resources appropriately.

## 2.5 Learner Activities

### Activity 1: Apply Linear Search

Given the list:

`[11, 4, 15, 7, 9]`

Use linear search to find `7`.

1. Write down each value you check.
2. How many elements do you check before finding the target?
3. How many elements would you check if the target were `12`, which is not in the list?

### Activity 2: Apply Binary Search

Given the sorted list:

`[2, 4, 6, 8, 10, 12, 14, 16]`

Use binary search to find `10`.

1. Which element do you check first?
2. Which part of the list can you eliminate?
3. Continue until you find the target.

### Activity 3: Apply Bubble Sort

Sort the following list in ascending order using bubble sort:

`[6, 3, 5, 2]`

Show the list after each complete pass.

### Activity 4: Apply Selection Sort

Sort the following list in ascending order using selection sort:

`[8, 4, 6, 2]`

Show the list after each pass and identify the smallest element selected each time.

### Activity 5: Choose the Best Method

For each situation, choose linear search or binary search and explain your choice.

1. You need to find a name in a short list that is not sorted.
2. You need to search a large list of numbers that is already sorted.
3. You need to find an item in an unsorted collection, and sorting the entire collection first would add unnecessary work.

### Suggested Answers

**Activity 1**

1. Check `11`, `4`, then `15`, and finally `7`.
2. Four elements.
3. All five elements, because `12` is not present.

**Activity 2**

1. Check `8`, the middle element chosen in the first step.
2. Since `10` is greater than `8`, eliminate the lower part.
3. Check `12`. Since `10` is smaller than `12`, continue with the lower part of the remaining search area and find `10`.

**Activity 3**

- Original: `[6, 3, 5, 2]`
- After Pass 1: `[3, 5, 2, 6]`
- After Pass 2: `[3, 2, 5, 6]`
- After Pass 3: `[2, 3, 5, 6]`

**Activity 4**

- Original: `[8, 4, 6, 2]`
- After Pass 1, select `2`: `[2, 4, 6, 8]`
- After Pass 2, select `4`: `[2, 4, 6, 8]`
- After Pass 3, select `6`: `[2, 4, 6, 8]`

**Activity 5**

1. Linear search, because the list is short and unsorted.
2. Binary search, because the list is sorted and may be large.
3. Linear search, because sorting the collection first may require more work than searching it directly.

## Key Takeaways

- Linear search checks elements one by one and works with sorted or unsorted data.
- Binary search repeatedly halves the search area and requires sorted data.
- Bubble sort compares adjacent elements and swaps them when they are in the wrong order.
- Selection sort repeatedly selects the smallest remaining element and places it in the correct position.
- Linear search has `O(n)` worst-case time complexity, binary search has `O(log n)`, and standard bubble sort and selection sort have `O(n²)` average and worst-case time complexity.
- Choosing an appropriate algorithm depends on the data, the task, and the resources available.

## References

1. Khan Academy, [Algorithms](https://en.khanacademy.org/computing/computer-science/algorithms).
2. MIT OpenCourseWare, [Introduction to Algorithms — Lecture Notes](https://ocw.mit.edu/courses/6-006-introduction-to-algorithms-fall-2011/pages/lecture-notes/).
3. Khan Academy, [Binary Search](https://www.khanacademy.org/computing/computer-science/algorithms/binarysearch/a/binary-search).
