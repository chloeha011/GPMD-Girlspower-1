# TEST BANK — PART A: TRUE OR FALSE

**Team:** GPMD  
**Module:** Algorithms, Data Structures & Connectionist AI  
**Assessment:** 30 Questions

## Instructions

Read each statement carefully and determine whether it is true or false. Circle or mark one answer for each question. Complete all questions before consulting the answer key.

Each question includes a Study Guide chapter reference.

## Questions

**TF01** [Guide §1] An algorithm must have sufficiently clear steps and a defined stopping condition.  
**True / False**

**TF02** [Guide §1] Pseudocode must follow the syntax of a particular programming language.  
**True / False**

**TF03** [Guide §1] A condition can determine which branch of an algorithm is executed.  
**True / False**

**TF04** [Guide §2] Linear search only works if the input list is sorted.  
**True / False**

**TF05** [Guide §2] Binary search can discard half a search range because the data is ordered.  
**True / False**

**TF06** [Guide §2] For an unsorted list, binary search always returns the correct answer.  
**True / False**

**TF07** [Guide §2] The worst-case runtime of linear search grows as O(n).  
**True / False**

**TF08** [Guide §3] Bubble sort repeatedly compares adjacent elements.  
**True / False**

**TF09** [Guide §3] Selection sort always chooses the largest remaining value for the front when sorting in ascending order.  
**True / False**

**TF10** [Guide §3] A conventional insertion sort builds an ordered prefix.  
**True / False**

**TF11** [Guide §3] Standard selection sort has O(log n) worst-case time complexity.  
**True / False**

**TF12** [Guide §4] Big O notation is an exact measurement of elapsed seconds on a specific laptop.  
**True / False**

**TF13** [Guide §4] O(n²) dominant work grows about fourfold when n doubles.  
**True / False**

**TF14** [Guide §4] Auxiliary space includes the storage already occupied by the input.  
**True / False**

**TF15** [Guide §4] An algorithm can exchange faster execution for greater additional memory use.  
**True / False**

**TF16** [Guide §5] An array typically supports constant-time access by valid index.  
**True / False**

**TF17** [Guide §5] A singly linked list provides constant-time access to its 100th node by index.  
**True / False**

**TF18** [Guide §5] A stack removes the most recently pushed element first.  
**True / False**

**TF19** [Guide §5] A FIFO queue removes the newest item first.  
**True / False**

**TF20** [Guide §5] A linked-list insertion can take O(1) time when the relevant predecessor node is already available.  
**True / False**

**TF21** [Guide §6] An ordinary non-empty tree with n nodes has n−1 edges.  
**True / False**

**TF22** [Guide §6] A general graph must contain one root and no cycles.  
**True / False**

**TF23** [Guide §6] Breadth-First Search (BFS) typically explores nodes using a queue.  
**True / False**

**TF24** [Guide §6] BFS always finds the least-cost route even when edge costs differ.  
**True / False**

**TF25** [Guide §7] Connectionist AI can learn patterns by adjusting numerical weights from data.  
**True / False**

**TF26** [Guide §7] An artificial neural network is a biologically exact copy of a human brain.  
**True / False**

**TF27** [Guide §7] Supervised learning examples include target labels.  
**True / False**

**TF28** [Guide §8] Forward propagation by itself updates all the model weights.  
**True / False**

**TF29** [Guide §8] Backpropagation calculates gradients used by an optimizer.  
**True / False**

**TF30** [Guide §8] A low loss on training data guarantees correct predictions on unseen cases.  
**True / False**

---

## Answer Key with Explanations

| Question | Answer | Explanation |
|---|---|---|
| TF01 | **True** | A finite, well-specified procedure must say when it terminates. |
| TF02 | **False** | Pseudocode expresses logic without requiring formal programming-language syntax. |
| TF03 | **True** | A condition selects an action based on a test. |
| TF04 | **False** | Linear search can examine either sorted or unsorted collections. |
| TF05 | **True** | Ordering supports discarding values known to be too high or too low. |
| TF06 | **False** | Standard binary search depends on sorted input. |
| TF07 | **True** | It may inspect every one of the n elements. |
| TF08 | **True** | Adjacent comparisons and swaps are its defining operations. |
| TF09 | **False** | The ascending-order variant chooses the smallest value in the unsorted section. |
| TF10 | **True** | Each new item is inserted into the previously sorted prefix. |
| TF11 | **False** | Standard selection sort performs a quadratic number of comparisons: O(n²). |
| TF12 | **False** | Big O describes asymptotic growth rather than elapsed clock time. |
| TF13 | **True** | (2n)² = 4n², ignoring lower-order terms. |
| TF14 | **False** | Auxiliary space excludes storage of the input itself. |
| TF15 | **True** | Time–space trade-offs are common in algorithm design. |
| TF16 | **True** | A conventional array calculates an element's address from its index. |
| TF17 | **False** | Finding a later node normally requires following links, taking O(n) time. |
| TF18 | **True** | A stack follows the Last In, First Out (LIFO) principle. |
| TF19 | **False** | A FIFO queue removes the earliest enqueued item first. |
| TF20 | **True** | Relinking a constant number of pointers is sufficient in this case. |
| TF21 | **True** | A connected, acyclic tree has exactly one fewer edge than vertices. |
| TF22 | **False** | Graphs do not require a root and may contain cycles. |
| TF23 | **True** | Its FIFO frontier visits vertices level by level. |
| TF24 | **False** | BFS minimizes the number of edges in an unweighted or equal-cost graph, not arbitrary weighted cost. |
| TF25 | **True** | Training modifies the strength of weighted connections. |
| TF26 | **False** | An artificial neural network is a mathematical model with broad biological inspiration, not an exact brain copy. |
| TF27 | **True** | Labels supply desired outputs for supervised training. |
| TF28 | **False** | A forward pass computes predictions; an optimizer updates parameters later. |
| TF29 | **True** | Backpropagation applies the chain rule to calculate derivatives of the loss. |
| TF30 | **False** | Generalization must be evaluated separately on unseen data. |

---

**End of Part A — True or False**
