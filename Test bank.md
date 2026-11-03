
# TEST BANK
## 70 Challenges to Test Your Thinking — With Explained Answers

**Team:** GPMD  
**Module:** Algorithms, Data Structures & Connectionist AI

**30 TRUE / FALSE • 30 MULTIPLE CHOICE • 10 EXTENDED RESPONSES**

---

## INSTRUCTIONS

Complete all questions before consulting the answer key.

- **True/False:** Circle one answer.
- **Multiple Choice:** Select exactly ONE answer (A–D) per item.
- **Extended Response:** Normally write at least 100 words or provide equivalent clear diagrams, calculations, or worked steps.

All necessary information is supplied below. Each question shows its Study Guide chapter reference.

## QUESTION OVERVIEW

| Section | Question Numbers | Count |
|---|---|---:|
| True/False | TF01–TF30 | 30 |
| Multiple Choice | MC01–MC30 | 30 |
| Extended Response | OE01–OE10 | 10 |
| **TOTAL** | **TF01–OE10** | **70** |

---

# PART A — TRUE OR FALSE

**TF01** [Guide §1] An algorithm must have sufficiently clear steps and a defined stopping condition.  
True / False

**TF02** [Guide §1] Pseudocode must follow the syntax of a particular programming language.  
True / False

**TF03** [Guide §1] A condition can determine which branch of an algorithm is executed.  
True / False

**TF04** [Guide §2] Linear search only works if the input list is sorted.  
True / False

**TF05** [Guide §2] Binary search can discard half a search range because the data is ordered.  
True / False

**TF06** [Guide §2] For an unsorted list, binary search always returns the correct answer.  
True / False

**TF07** [Guide §2] The worst-case runtime of linear search grows as O(n).  
True / False

**TF08** [Guide §3] Bubble sort repeatedly compares adjacent elements.  
True / False

**TF09** [Guide §3] Selection sort always chooses the largest remaining value for the front when sorting ascending.  
True / False

**TF10** [Guide §3] A conventional insertion sort builds an ordered prefix.  
True / False

**TF11** [Guide §3] Standard selection sort has O(log n) worst-case time complexity.  
True / False

**TF12** [Guide §4] Big O notation is an exact measurement of elapsed seconds on a specific laptop.  
True / False

**TF13** [Guide §4] O(n²) dominant work grows about fourfold when n doubles.  
True / False

**TF14** [Guide §4] Auxiliary space includes the storage already occupied by the input.  
True / False

**TF15** [Guide §4] An algorithm can exchange faster execution for greater additional memory use.  
True / False

**TF16** [Guide §5] An array typically supports constant-time access by valid index.  
True / False

**TF17** [Guide §5] A singly linked list provides constant-time access to its 100th node by index.  
True / False

**TF18** [Guide §5] A stack removes the most recently pushed element first.  
True / False

**TF19** [Guide §5] A FIFO queue removes the newest item first.  
True / False

**TF20** [Guide §5] A linked-list insertion can take O(1) time when the relevant predecessor node is already available.  
True / False

**TF21** [Guide §6] An ordinary non-empty tree with n nodes has n−1 edges.  
True / False

**TF22** [Guide §6] A general graph must contain one root and no cycles.  
True / False

**TF23** [Guide §6] BFS typically explores nodes using a queue.  
True / False

**TF24** [Guide §6] BFS always finds the least-cost route even when edge costs differ.  
True / False

**TF25** [Guide §7] Connectionist AI can learn patterns by adjusting numerical weights from data.  
True / False

**TF26** [Guide §7] An artificial neural network is a biologically exact copy of a human brain.  
True / False

**TF27** [Guide §7] Supervised learning examples include target labels.  
True / False

**TF28** [Guide §8] Forward propagation by itself updates all the model weights.  
True / False

**TF29** [Guide §8] Backpropagation calculates gradients used by an optimizer.  
True / False

**TF30** [Guide §8] A low loss on training data guarantees correct predictions on unseen cases.  
True / False

---

# PART B — MULTIPLE-CHOICE QUESTIONS

**MC01** [Guide §1] Which component tells an algorithm what it receives?

A. Output  
B. Input  
C. Loop  
D. Condition

**MC02** [Guide §1] Which is the clearest stopping rule for finding a name in a list?

A. Stop when bored  
B. Stop once a match is found or all names have been checked  
C. Always check exactly two names  
D. Stop before comparing anything

**MC03** [Guide §2] Trace linear search for 7 in [3,6,7,2]. How many comparisons occur?

A. 1  
B. 2  
C. 3  
D. 4

**MC04** [Guide §2] With lower-middle convention, search for 10 in sorted [2,4,6,8,10,12,14,16]. Which values are inspected?

A. 8,12,10  
B. 10 only  
C. 8,6,10  
D. 12,14,10

**MC05** [Guide §2] Which search requires sorted data for its usual correctness guarantee?

A. Linear search  
B. Binary search  
C. Checking every item  
D. Random scan

**MC06** [Guide §3] After the first bubble-sort pass over [5,3,8,2], what is the list?

A. [2,3,5,8]  
B. [3,5,2,8]  
C. [3,2,5,8]  
D. [5,2,3,8]

**MC07** [Guide §3] After the first selection-sort pass over [5,3,8,2], what is the list?

A. [3,5,8,2]  
B. [5,3,2,8]  
C. [2,3,8,5]  
D. [2,5,3,8]

**MC08** [Guide §3] Which method grows a sorted prefix by inserting one item at a time?

A. Insertion sort  
B. Selection sort  
C. Binary search  
D. Breadth-first search

**MC09** [Guide §3] Which modification can make bubble sort stop early on already sorted input?

A. Always swap once  
B. Stop if a complete pass makes zero swaps  
C. Use binary search  
D. Select the minimum on each pass

**MC10** [Guide §4] Which is the correct asymptotic worst-case time of standard selection sort?

A. O(1)  
B. O(log n)  
C. O(n)  
D. O(n²)

**MC11** [Guide §4] How does dominant O(n) work change when n doubles?

A. It doubles  
B. It quadruples  
C. It stays fixed  
D. It is halved

**MC12** [Guide §4] Which category best describes binary-search time?

A. O(n²)  
B. O(2ⁿ)  
C. O(log n)  
D. O(n log n)

**MC13** [Guide §4] Which term means memory beyond the provided input?

A. Wall-clock time  
B. Auxiliary space  
C. Output label  
D. Index value

**MC14** [Guide §4] Why can a lower Big O class still run slower on a small input?

A. Asymptotics predict exact milliseconds  
B. Hardware speed is irrelevant  
C. Constants and implementation overhead matter  
D. Worst cases never happen

**MC15** [Guide §5] What is a[2] for a=[85,92,78,90] in zero-based indexing?

A. 85  
B. 92  
C. 78  
D. 90

**MC16** [Guide §5] After pushing A, B, C onto a stack, what does pop() return?

A. A  
B. B  
C. C  
D. None

**MC17** [Guide §5] A FIFO queue starts [A,B,C]. After one dequeue and enqueue(D), what remains?

A. [D,B,C]  
B. [B,C,D]  
C. [A,B,D]  
D. [D,C,B]

**MC18** [Guide §5] Which structure suits a text editor’s undo history?

A. Stack  
B. Queue  
C. Graph  
D. Adjacency matrix

**MC19** [Guide §5] What is typically needed for O(1) insertion after a node in a singly linked list?

A. A sorted array  
B. The predecessor/current node reference  
C. The total list length  
D. A hash of every element

**MC20** [Guide §6] Which property describes a tree?

A. Every vertex has a cycle  
B. Connected and acyclic  
C. All edges are directed outward by definition  
D. All nodes have exactly two children

**MC21** [Guide §6] Which are the leaves in a tree with root 10, children 5 and 15, and children 2 and 7 under 5?

A. 10,5  
B. 5,15  
C. 2,7,15  
D. 10,2,7

**MC22** [Guide §6] What is preorder for that same tree?

A. 2,5,7,10,15  
B. 10,5,2,7,15  
C. 2,7,5,15,10  
D. 10,15,7,2,5

**MC23** [Guide §6] What structure does BFS normally use for its frontier?

A. Stack  
B. Queue  
C. Sorted array of weights  
D. Binary search tree

**MC24** [Guide §6] Which representation stores a square table of vertex pair connections?

A. Adjacency matrix  
B. Stack  
C. Trie  
D. Linked-list head

**MC25** [Guide §7] What is the purpose of a hidden layer?

A. Store the external file  
B. Compute learned intermediate representations  
C. Guarantee interpretability  
D. Replace all training labels

**MC26** [Guide §7] Which is an example of supervised training?

A. Cluster unlabeled customers  
B. Learn labels from labeled spam messages  
C. Randomly shuffle a queue  
D. Read an unsorted list

**MC27** [Guide §8] For x1=2, x2=1, w1=0.5, w2=−0.2 and b=0.1, what is z?

A. 0.5  
B. 0.7  
C. 0.9  
D. 1.3

**MC28** [Guide §8] For z=−3, what does ReLU return?

A. −3  
B. 0  
C. 1  
D. 3

**MC29** [Guide §8] If weight=0.5, gradient=0.4, learning rate=0.1, what is the new weight?

A. 0.54  
B. 0.46  
C. 0.40  
D. 0.90

**MC30** [Guide §8] Which best tests whether a trained classifier generalizes?

A. Report training loss alone  
B. Evaluate on separate unseen labeled examples  
C. Count number of layers only  
D. Assume no mistakes after 100 epochs

---

# PART C — EXTENDED-RESPONSE QUESTIONS

**OE01** [Guide §1–2] Write clear pseudocode to search for one student ID in an unsorted list. Explain its input, output, stopping rule, best and worst case. Then explain when binary search becomes an option.

**OE02** [Guide §2–3] Trace binary search for 10 in [2,4,6,8,10,12,14,16], using the lower middle for even-length ranges. Trace one complete bubble-sort pass on [6,3,5,2]. Compare the two procedures and their objectives.

**OE03** [Guide §3–4] Sort [6,3,5,2] using selection sort and insertion sort, showing intermediate arrays. Explain why either might be chosen for small inputs despite O(n²) worst-case behavior.

**OE04** [Guide §4] A project grows from 100 to 1,000,000 records. Compare O(log n), O(n) and O(n²) growth using a table or calculations. Discuss why Big O is not a direct runtime benchmark and identify a possible time–space trade-off.

**OE05** [Guide §5] Design the data-storage part of a student portal: grades, undo actions, arrivals and a frequently changing linked chain. Choose structures, justify common operation costs, and give a case where your choice would be inconvenient.

**OE06** [Guide §5] Given stack operations push(A), push(B), push(C), pop(), push(D), peek(), and queue operations enqueue(A), enqueue(B), enqueue(C), dequeue(), enqueue(D): show each intermediate state, return values, and explain LIFO versus FIFO.

**OE07** [Guide §6] For root 10 with children 5 and 15, and children 2 and 7 under 5, identify root, leaves, depth of node 7, and preorder/inorder/postorder visits. Explain the difference between a tree and a general graph.

**OE08** [Guide §6] On undirected graph edges A–B, A–C, B–D and C–D, trace BFS from A to D exploring B before C. Show the queue; explain why its path is shortest in edge count and why different costs change the guarantee.

**OE09** [Guide §7] Compare a rule-based spam filter and a connectionist spam classifier, covering how each is built, an example error, data requirements, interpretability and how you would evaluate them.

**OE10** [Guide §8–9] Explain a complete neural-network training cycle using the equation z=Σw_ix_i+b, activation, loss, backpropagation and optimizer updates. Demonstrate a weight update with w=0.5, gradient=0.4, learning rate=0.1; then explain generalization and one responsible-use concern.

---

# ANSWER KEY

## PART A — TRUE OR FALSE

**TF01 — TRUE.** A finite, well-specified procedure must say when it terminates.

**TF02 — FALSE.** Pseudocode expresses logic without requiring formal programming-language syntax.

**TF03 — TRUE.** A condition selects an action based on a test.

**TF04 — FALSE.** Linear search can examine either sorted or unsorted collections.

**TF05 — TRUE.** The ordering supports discarding values known to be too high or too low.

**TF06 — FALSE.** Standard binary search depends on sorted input.

**TF07 — TRUE.** It may inspect every one of the n elements.

**TF08 — TRUE.** Adjacent comparisons and swaps are its defining operation.

**TF09 — FALSE.** The ascending-order variant chooses the smallest value in the unsorted suffix.

**TF10 — TRUE.** Each new item is inserted into the previously sorted prefix.

**TF11 — FALSE.** It performs a quadratic number of comparisons, O(n²), in standard form.

**TF12 — FALSE.** It describes asymptotic growth rather than elapsed clock time.

**TF13 — TRUE.** (2n)²=4n², ignoring lower-order terms.

**TF14 — FALSE.** Auxiliary space excludes storage of the input itself.

**TF15 — TRUE.** Time–space trade-offs are common.

**TF16 — TRUE.** A conventional array computes an element address from its index.

**TF17 — FALSE.** Finding a later node normally requires following links, O(n).

**TF18 — TRUE.** A stack obeys LIFO.

**TF19 — FALSE.** It removes the earliest enqueued item first.

**TF20 — TRUE.** Relinking a constant number of pointers suffices in that case.

**TF21 — TRUE.** Connected acyclic trees have exactly one fewer edge than vertices.

**TF22 — FALSE.** Graphs need not have a root and may contain cycles.

**TF23 — TRUE.** Its FIFO frontier visits vertices level by level.

**TF24 — FALSE.** It minimizes the number of edges in an unweighted/equal-cost graph, not arbitrary weighted cost.

**TF25 — TRUE.** Training modifies the strength of weighted connections.

**TF26 — FALSE.** It is a mathematical model with only broad biological inspiration.

**TF27 — TRUE.** Labels supply desired outputs for supervised training.

**TF28 — FALSE.** A forward pass computes predictions; an optimizer updates parameters later.

**TF29 — TRUE.** It applies the chain rule to compute derivatives of loss.

**TF30 — FALSE.** Generalization must be evaluated separately on unseen data.

---

## PART B — MULTIPLE-CHOICE ANSWERS

| Question | Answer | Explanation |
|---|---|---|
| MC01 | **B** | Input is the data given to the procedure. |
| MC02 | **B** | It covers both found and absent cases. |
| MC03 | **C** | It checks 3, 6 and 7. |
| MC04 | **A** | The midpoint checks are 8, then 12, then 10. |
| MC05 | **B** | Discarding half is valid only if values are ordered. |
| MC06 | **B** | Adjacent swaps move 8 to the end: [3,5,2,8]. |
| MC07 | **C** | Minimum 2 swaps with first value 5. |
| MC08 | **A** | Insertion sort grows its ordered prefix. |
| MC09 | **B** | A pass with no swaps establishes sorted order. |
| MC10 | **D** | Nested scanning yields quadratic comparisons. |
| MC11 | **A** | A linear term is proportional to n. |
| MC12 | **C** | Each step shrinks the remaining range by about half. |
| MC13 | **B** | Auxiliary space excludes input storage. |
| MC14 | **C** | Lower growth rates do not settle all small-input timings. |
| MC15 | **C** | Index 2 refers to the third element. |
| MC16 | **C** | The last pushed item C is on top. |
| MC17 | **B** | A leaves the front and D joins the rear. |
| MC18 | **A** | Undo most often reverses the latest action first. |
| MC19 | **B** | Known insertion location avoids traversal. |
| MC20 | **B** | The underlying ordinary tree is connected with no cycles. |
| MC21 | **C** | These vertices have no children. |
| MC22 | **B** | Preorder visits root, left subtree then right subtree. |
| MC23 | **B** | FIFO supports level-by-level exploration. |
| MC24 | **A** | An adjacency matrix indexes source/destination vertex pairs. |
| MC25 | **B** | Hidden units transform intermediate features. |
| MC26 | **B** | Spam versus not-spam labels supply targets. |
| MC27 | **C** | (2×0.5) +(1×−0.2) +0.1=0.9. |
| MC28 | **B** | ReLU is max (0, z). |
| MC29 | **B** | 0.5−0.1×0.4=0.46. |
| MC30 | **B** | Unseen test examples reveal performance beyond memorized training cases. |

---

## PART C — EXTENDED-RESPONSE MODEL ANSWERS

### OE01 — Model Answer

Input: list L and target t. Output: first matching position, or not-found.

Pseudocode:

```text
FOR i from 0 to length(L) - 1:
    IF L[i] equals t:
        RETURN i

RETURN not-found
```

The loop has an explicit endpoint, works on unsorted data, and gives O(1) best-case comparisons and O(n) worst-case comparisons. If the list is already sorted and supports efficient indexed access, binary search can choose a middle entry and discard a half on each comparison, O(log n) time. Sorting once merely to answer one small lookup may not be worthwhile.

### OE02 — Model Answer

Binary search checks 8, then 12, then 10, under the stated lower-middle convention.

For bubble sort [6,3,5,2]:

1. Compare 6–3 → [3,6,5,2]
2. Compare 6–5 → [3,5,6,2]
3. Compare 6–2 → [3,5,2,6]

A search identifies a target in data; a sort changes the data order. Binary search needs ordered input, while bubble sort can reorder arbitrary input by swapping adjacent elements. Binary search is O(log n) in its conventional indexed implementation, while standard bubble sort is O(n²) average and worst case.

### OE03 — Model Answer

**Selection sort:**

[6,3,5,2] → [2,3,5,6] (select 2) → [2,3,5,6] (select 3) → [2,3,5,6] (select 5).

**Insertion sort:**

- Sorted prefix starts [6].
- Insert 3 → [3,6,5,2].
- Insert 5 → [3,5,6,2].
- Insert 2 → [2,3,5,6].

Both are understandable, easy to implement and practical on small inputs. Insertion sort can work especially well on nearly ordered data; selection sort performs few swaps while continuing to scan for the minimum.

### OE04 — Model Answer

Ignoring constants, for n=100 versus 1,000,000:

| Complexity | n = 100 | n = 1,000,000 |
|---|---:|---:|
| O(log n) | About 6.64 | About 19.93 |
| O(n) | 100 | 1,000,000 |
| O(n²) | 10,000 | 1,000,000,000,000 |

Big O models growth under assumptions; it does not provide clock times or account for constant costs, caches, language or input patterns. A time–space trade-off might be an auxiliary index that speeds lookup at the cost of additional memory, or array merge sort with O(n log n) time and O(n) auxiliary space.

### OE05 — Model Answer

Use an array/list for grades requiring indexed access, a stack for undo because most recent changes are reversed first, a FIFO queue for students waiting for service, and a linked list for a chain where insertions at known positions are frequent.

Array indexed access is usually O(1), but middle insertions may require O(n) shifts. Stack push/pop and queue enqueue/dequeue are generally O(1) with suitable implementations. Linked-list insertion can be O(1) when its predecessor is known, but locating a node by position is O(n). If arrival requests had priority classes, a plain FIFO queue may not meet the requirements.

### OE06 — Model Answer

**Stack:**

[] → [A] → [A, B] → [A, B, C] → pop returns C, leaving [A, B] → push D gives [A, B, D] → peek returns D without removal.

**Queue:**

[] → [A] → [A, B] → [A, B, C] → dequeue returns A, leaving [B, C] → enqueue D gives [B, C, D].

The stack removes the newest entry (LIFO) and is suitable for undo; the queue removes the earliest entry (FIFO) and is suitable for ordinary arrival-order service. The same input sequence therefore produces different returned values.

### OE07 — Model Answer

Root is 10. Leaves are 2, 7 and 15; 7 is at depth 2 if depth counts edges from the root.

- **Preorder:** 10,5,2,7,15.
- **Inorder:** 2,5,7,10,15.
- **Postorder:** 2,7,5,15,10.

In this rooted tree each non-root node has one parent and the graph is connected and acyclic. A general graph may have cycles, arbitrary degrees and multiple routes, and need not have a root. A tree with five nodes has four edges.

### OE08 — Model Answer

Initialize queue [A].

1. Remove A and discover B, C → [B, C].
2. Remove B, discover D → [C, D].
3. Remove C; D already discovered → [D].
4. Remove D, reached goal → [].

With parent references, path A→B→D has two edges. A→C→D also uses two edges. BFS explores by edge distance, so first discovery yields the fewest edges when edges are equal cost. If corridor costs differ, the fewest-edge path may be expensive; a cost-aware shortest-path procedure is needed.

### OE09 — Model Answer

A rule-based spam filter can check manually selected words or sender fields; its rules are easy to inspect but miss exceptions and may flag legitimate messages.

A connectionist classifier processes numerical email features and learns weights from labelled spam and non-spam examples. It can capture combinations not covered by short rules, but its decisions can be hard to explain and may reflect dataset bias.

Compare both systems on separate unseen labelled messages and report false positives, false negatives and appropriate summary metrics. Training accuracy alone is insufficient. Neither system is automatically perfect or appropriate for all situations.

### OE10 — Model Answer

A neuron computes:

\[
z = \sum w_i x_i + b
\]

It then produces an output \(a=f(z)\), perhaps with ReLU or sigmoid.

A forward pass produces a prediction. A loss function scores how it differs from the target. Backpropagation computes gradients of loss with respect to weights/biases using the chain rule.

An optimizer such as gradient descent updates them:

\[
w_{\text{new}} = w - \eta g
\]

\[
w_{\text{new}} = 0.5 - (0.1 \times 0.4) = 0.46
\]

Iterating over examples and epochs can lower training loss, but unseen labelled cases are needed to evaluate generalization. An unrepresentative dataset can produce biased predictions; therefore, data quality, limitations, and human oversight matter.

---

**END OF TEST BANK**

*GPMD — Algorithms, Data Structures & Connectionist AI*
