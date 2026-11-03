# Terminology: Algorithms

This section introduces important terms related to algorithms. Each term is explained in simple language, with examples to help beginners understand how algorithms work.

## 1. Algorithm

An **algorithm** is a set of clear, ordered instructions used to solve a problem or complete a task.

**Example:** A recipe is similar to an algorithm because it provides steps that must be followed to prepare a meal.

## 2. Searching Algorithm

A **searching algorithm** is a method used to find a specific item in a collection of data.

**Example:** Finding a student's name in a class list.

## 3. Sorting Algorithm

A **sorting algorithm** arranges data in a particular order, such as from smallest to largest or alphabetically.

**Example:** Arranging student scores from highest to lowest.

## 4. Linear Search

**Linear search** checks each item in a collection one by one until the target is found or there are no more items to check. It works with both sorted and unsorted data.

**Example:** To find `8` in `[2, 5, 8, 12, 16]`, linear search checks `2`, then `5`, and finally `8`.

## 5. Binary Search

**Binary search** finds an item by repeatedly dividing a sorted collection into smaller halves. It checks the middle value and continues searching in the half that may contain the target.

**Example:** To find `12` in `[2, 5, 8, 12, 16]`, binary search checks `8` first and then searches the right half.

**Important:** Binary search only works correctly when the data is sorted.

## 6. Bubble Sort

**Bubble sort** repeatedly compares neighboring elements and swaps them when they are in the wrong order. This process continues until the collection is sorted.

**Example:** `[5, 2, 4]` becomes `[2, 4, 5]` after the elements are compared and swapped as needed.

## 7. Selection Sort

**Selection sort** repeatedly finds the smallest element in the unsorted part of a collection and places it at the beginning of that part.

**Example:** When sorting `[5, 2, 4]`, selection sort first finds `2` and places it at the beginning.

## 8. Input

**Input** is the information or data given to an algorithm to process.

**Example:** In an algorithm that adds two numbers, `5` and `3` are the inputs.

## 9. Output

**Output** is the result produced after an algorithm processes its input.

**Example:** If an algorithm adds `5` and `3`, the output is `8`.

## 10. Pseudocode

**Pseudocode** describes an algorithm using simple, structured language instead of the exact rules of a programming language. It helps people plan their solutions before writing code.

**Example:**

1. Start.
2. Read two numbers.
3. Add the numbers.
4. Display the result.
5. Stop.

## 11. Condition

A **condition** is a rule that determines what an algorithm should do in a particular situation. It is commonly used with instructions such as `if` and `else`.

**Example:** If a number is greater than `10`, display "Large". Otherwise, display "Small or equal to 10".

## 12. Loop

A **loop** repeats a set of instructions until a condition is met or a specified number of repetitions is completed.

**Example:** An algorithm can use a loop to check every number in a list.

## 13. Time Complexity

**Time complexity** describes how the amount of work an algorithm performs grows as the input size increases. It helps us compare how efficiently different algorithms solve a problem.

**Example:** Linear search may check every item, while binary search repeatedly halves the search area when the data is sorted.

## 14. Space Complexity

**Space complexity** describes how the amount of memory an algorithm needs grows as the input size increases.

**Example:** An algorithm that creates a new list to store its results may need more memory as the input becomes larger.

## 15. Auxiliary Space

**Auxiliary space** is the extra memory an algorithm uses while running, not including the memory needed to store the original input.

**Example:** If an algorithm creates a temporary list to organize data, that list uses auxiliary space.

## 16. Efficiency

**Efficiency** describes how well an algorithm uses resources, such as time and memory, to complete a task.

**Example:** An algorithm that finds an item using fewer comparisons may be more efficient than one that checks every item.

## 17. Big O Notation

**Big O notation** describes how an algorithm's time or memory requirements grow as the input size increases. It helps us understand and compare algorithm efficiency.

Common examples include:

- `O(1)`: Constant growth — the amount of work stays roughly the same as the input grows.
- `O(log n)`: Logarithmic growth — the amount of work grows slowly as the input increases.
- `O(n)`: Linear growth — the amount of work grows in proportion to the input size.
- `O(n²)`: Quadratic growth — the amount of work can grow much faster as the input size increases.

**Example:** Linear search has a worst-case time complexity of `O(n)`, while binary search has a worst-case time complexity of `O(log n)`.

## 18. Best Case, Average Case, and Worst Case

These terms describe how an algorithm performs under different situations.

- **Best case:** The situation where an algorithm requires the least amount of work.
- **Average case:** The expected amount of work across typical inputs, based on an assumed distribution of possible inputs.
- **Worst case:** The situation where an algorithm requires the most amount of work.

**Example:** In linear search:
- Best case: The target is the first element.
- Average case: The target is somewhere in the middle of the collection.
- Worst case: The target is the last element or is not present.

## 19. Time-Space Trade-off

A **time-space trade-off** occurs when an algorithm uses more memory to reduce the time needed to complete a task, or uses less memory but takes more time.

**Example:** An algorithm may store previously calculated results in memory so that it does not need to calculate them again.

## 20. Benchmarking

**Benchmarking** is the process of testing an algorithm or program to measure its actual performance, such as execution time and memory usage.

**Example:** Running two sorting algorithms on the same dataset and comparing how long they take to finish.

## References

1. **NIST — Dictionary of Algorithms and Data Structures**  
   https://xlinux.nist.gov/dads/  
   A reference for definitions and terminology related to algorithms and data structures.

2. **OpenDSA — Data Structures and Algorithms**  
   https://opendsa.org/  
   Learning materials covering algorithms, data structures, and their applications.

3. **Khan Academy — Algorithms**  
   https://www.khanacademy.org/computing/computer-science/algorithms  
   Beginner-friendly explanations of algorithms, searching, sorting, and efficiency.

4. **MIT OpenCourseWare — Introduction to Algorithms (6.006)**  
   https://ocw.mit.edu/courses/6-006-introduction-to-algorithms-spring-2020/  
   Additional lecture materials on algorithm design and analysis.
