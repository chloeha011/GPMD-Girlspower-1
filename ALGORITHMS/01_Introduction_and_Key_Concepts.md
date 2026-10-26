# Algorithms

## 1.1 What Is an Algorithm?

An **algorithm** is a sequence of clear, ordered instructions used to solve a problem or complete a task. It describes what steps should be followed, in what order, and when the process should stop.

Algorithms are not limited to computer science. We use them in everyday life, sometimes without even realizing it.

For example, imagine making a cup of tea:

1. Fill a kettle with water.
2. Heat the water until it boils.
3. Place a tea bag in a cup.
4. Pour the hot water into the cup.
5. Wait a few minutes.
6. Remove the tea bag.

These steps form an algorithm because they provide an organized way to complete a task. If the steps are unclear or performed in the wrong order, the result may not be what we expect.

In computer science, algorithms help computers solve problems such as searching for information, sorting data, calculating results, and recommending products or videos. Computers can process information quickly, but they still need instructions that tell them how to solve a problem.

### Characteristics of a Good Algorithm

A useful algorithm should have several important characteristics:

- **Clear instructions:** Each step should be specific and understandable.
- **Correctness:** It should produce the expected result when given valid input.
- **A definite ending:** It should finish after a finite number of steps.
- **A logical order:** The steps should be arranged so that the task can be completed correctly.

### Example: Finding a Student's Name

Imagine that a teacher has a list of student names and needs to find a particular student.

A simple algorithm could be:

1. Start with the first name on the list.
2. Compare it with the name you are looking for.
3. If the names match, report that the student has been found and stop.
4. If they do not match, move to the next name.
5. Repeat until the name is found or the list ends.
6. If the list ends without a match, report that the name was not found.

This is an example of a **linear search algorithm**. It checks items one by one until it finds the target or reaches the end of the list.

The same approach can be used to find a book in a collection, locate a product in a list, or search for a file on a computer.

## 1.2 Why Are Algorithms Important?

Algorithms help us solve problems systematically. Instead of relying on guesswork, we can follow a defined process and obtain results more consistently.

In everyday technology, algorithms are used in many ways. A map application calculates possible routes, an online store organizes products, and a video platform uses algorithms to help select content that may interest its users.

However, **different algorithms can solve the same problem with different levels of efficiency**. Some may require many steps, while others can reach the result with far fewer operations. Choosing an appropriate algorithm becomes especially important when working with large amounts of data.

### Example: Finding a Name in a List of 1,000 Students

Suppose you need to find one student's name in a list of 1,000 students.

**Method 1: Check Every Name**

You start at the beginning and compare each name with the target. This method works even if the names are not sorted. However, in the worst case, you may need to check all 1,000 names.

**Method 2: Repeatedly Divide the List in Half**

If the names are arranged alphabetically, you can use binary search:

1. Check the name in the middle of the list.
2. If the target comes alphabetically before it, continue with the first half.
3. If the target comes after it, continue with the second half.
4. Repeat until the name is found or no candidates remain.

Each comparison eliminates approximately half of the remaining candidates. For a sorted list of 1,000 names, binary search needs at most about 10 comparisons under the usual implementation, compared with up to 1,000 checks for linear search.

The important condition is that the list must already be sorted. Binary search cannot be applied directly to an unsorted list using this method.

This example shows that the way a problem is solved can matter just as much as the final result.

## 1.3 An Introduction to Searching Algorithms

A **searching algorithm** finds a particular item in a collection of data. The most suitable method depends on how the data is organized and how much data needs to be searched.

Two common examples are:

- **Linear search:** Checks items one by one. It is simple and works with both sorted and unsorted data.
- **Binary search:** Repeatedly divides the search area in half. It is efficient for sorted data because each comparison eliminates a large part of the remaining candidates.

For example, if you want to find a number in a short, unsorted list, linear search may be sufficient. If you need to search a large, sorted list repeatedly, binary search may be a better choice.

These two algorithms illustrate an important idea: the best approach depends on the problem and the conditions under which it must be solved.

The detailed steps and comparisons of searching algorithms are covered in the next section of the learning module.

## 1.4 An Introduction to Sorting Algorithms

A **sorting algorithm** arranges data in a particular order, such as from smallest to largest, from highest to lowest, or alphabetically.

Sorting makes data easier to read, compare, and sometimes search. For example, a teacher may sort student scores from highest to lowest, while an online store may sort products by price.

Different sorting algorithms organize data in different ways. One simple example is **insertion sort**, which builds a sorted section one element at a time.

Imagine arranging playing cards in your hand. You pick up one card and insert it into the correct position among the cards you have already arranged. Insertion sort follows a similar idea.

For example, consider the list:

`[5, 2, 8, 1]`

Using insertion sort, the list develops as follows:

1. Start with `5` as the sorted section.
2. Insert `2` before `5`: `[2, 5, 8, 1]`
3. Insert `8` into its correct position: `[2, 5, 8, 1]`
4. Insert `1` at the beginning: `[1, 2, 5, 8]`

The list is now arranged in ascending order.

Insertion sort is easy to understand and can work well for small or nearly sorted lists. However, it may require many movements when the list is large and randomly ordered.

More advanced sorting algorithms can be more suitable for larger collections. The choice depends on the amount of data and the requirements of the task.

## 1.5 Understanding Algorithm Efficiency

An algorithm should not only produce the correct answer; it should also use resources appropriately.

Two important aspects of efficiency are:

- **Time complexity:** Describes how the number of operations grows as the input size increases.
- **Space complexity:** Describes how the amount of additional memory required grows as the input size increases.

For example, checking a list of 10 names one by one may be quick enough. Doing the same with one million names may require much more work.

Computer scientists use **Big O notation**, such as `O(n)` and `O(log n)`, to describe how an algorithm's resource requirements grow as the input becomes larger.

You do not need to memorize every complexity formula at this stage. The key idea is that algorithms that seem similar on small examples may behave very differently when the amount of data increases.

The next section explores algorithm efficiency and compares how different algorithms perform as their input sizes grow.

## 1.6 Learner Activity: Choose an Appropriate Algorithm

Imagine that you are helping a teacher manage student records.

### Task 1: Searching

The student ID list is:

`[104, 108, 112, 116, 120, 124, 128]`

You need to find student ID `120`.

1. Would you choose linear search or binary search?
2. Show the values you would check and the order in which you would check them.
3. Explain why your chosen algorithm is suitable for this list.

### Task 2: Sorting

A teacher records four student scores:

`[75, 60, 90, 68]`

Use insertion sort to arrange the scores from smallest to largest. Show the list after each element is inserted into the correct position.

### Expected Answers

**Task 1:** Binary search is a suitable choice because the IDs are already sorted. Using the middle element of the seven-item list, first check `116`. Since `120` is greater, continue with the upper half, `[120, 124, 128]`. Check `124`, then search the lower part of that remaining range and find `120`.

**Task 2:**

- Initial list: `[75, 60, 90, 68]`
- Insert `60`: `[60, 75, 90, 68]`
- Insert `90`: `[60, 75, 90, 68]`
- Insert `68`: `[60, 68, 75, 90]`

### Reflection Questions

1. Why is it important for an algorithm to have clear instructions?
2. Why does binary search require sorted data?
3. Can two algorithms solve the same problem but have different levels of efficiency? Give an example.

## Key Takeaways

- An algorithm is a clear, ordered sequence of steps for solving a problem.
- Algorithms are used in everyday life as well as computer science.
- Linear search checks items one by one, while binary search repeatedly halves the search area in sorted data.
- Sorting algorithms arrange data into a chosen order.
- Algorithm efficiency concerns how time and memory requirements grow as the input size increases.
- A suitable algorithm depends on the problem, the data, and the available resources.

## References

1. Khan Academy, [Algorithms](https://en.khanacademy.org/computing/computer-science/algorithms).
2. MIT OpenCourseWare, [Introduction to Algorithms — Lecture Notes](https://ocw.mit.edu/courses/6-006-introduction-to-algorithms-fall-2011/pages/lecture-notes/).
3. Khan Academy, [Binary Search](https://www.khanacademy.org/computing/computer-science/algorithms/binarysearch/a/binary-search).
4. Khan Academy, [Insertion Sort](https://en.khanacademy.org/computing/computer-science/algorithms/insertion-sort/a/insertion-sort).
