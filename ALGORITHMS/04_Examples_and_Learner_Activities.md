# Algorithms: Examples and Learner Activities


## 1. Learning Objectives

After completing this section, learners should be able to trace simple algorithms, apply searching and sorting methods, and explain which method is more suitable for a given problem.

## 2. Worked Examples

### Example 1: Linear Search

Suppose we want to find `8` in the list `[3, 6, 8, 2, 9]`.

Linear search checks each item from left to right until it finds the target.

```text
[3] → [6] → [8] → [2] → [9]
 1     2     3
             ↑
          Found!
```

The algorithm checks `3`, then `6`, and finally `8`. The target is found at position 3, so the search stops.

### Example 2: Binary Search

Now find `12` in the sorted list `[2, 4, 6, 8, 10, 12, 14]`.

1. Check the middle value, `8`. Since `12` is larger, search the right half.
2. Check the middle of `[10, 12, 14]`, which is `12`.
3. The target is found.

Binary search reduces the search range at each step. Unlike linear search, it requires the data to be sorted.

### Example 3: Sorting with Selection Sort

Sort `[5, 3, 8, 2]` from smallest to largest.

| Step | Action | List |
|---|---|---|
| Start | Original list | `[5, 3, 8, 2]` |
| 1 | Find 2 and swap it with 5 | `[2, 3, 8, 5]` |
| 2 | The smallest remaining value is 3, already in place | `[2, 3, 8, 5]` |
| 3 | Find 5 and swap it with 8 | `[2, 3, 5, 8]` |

The final list is `[2, 3, 5, 8]`. Selection sort works by placing the smallest remaining item into its correct position.

## 3. Learner Activities

Try these questions before checking the answers below.

**Activity A — Linear Search**

Find `7` in `[4, 1, 7, 3, 9]`.

- Which items do you check?
- At what position is the target found?

**Activity B — Bubble Sort**

Sort `[4, 2, 5, 1]` in ascending order. Show the list after each swap in the first pass.

**Activity C — Choosing an Algorithm**

A school has 5,000 student IDs stored in sorted order. You need to find one ID.

- Would you choose linear search or binary search?
- Why?

## 4. Answers and Explanations

**Activity A:** Check `4`, then `1`, then `7`. The target is at position 3. Linear search stops as soon as it finds the target.

**Activity B:** Start with `[4, 2, 5, 1]`.

- Swap 4 and 2: `[2, 4, 5, 1]`
- Compare 4 and 5: no swap.
- Swap 5 and 1: `[2, 4, 1, 5]`

The first pass ends at `[2, 4, 1, 5]`. After the remaining passes, the sorted list is `[1, 2, 4, 5]`.

**Activity C:** Binary search is usually the better choice because it repeatedly halves the search range. The list must remain sorted for binary search to work correctly.

## 5. Key Takeaways

- Linear search checks items one by one.
- Binary search narrows the search range and requires sorted data.
- Sorting algorithms arrange data into a chosen order using different methods.
- The best algorithm depends on the problem, the data, and the required efficiency.

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

These resources are provided for further learning and verification. The team should check the relevant materials, confirm the examples and answers, and record the outcome of peer review before marking this file as checked.
