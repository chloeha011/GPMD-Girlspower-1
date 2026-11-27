# Resource Mapping (Stage 3, Updated)

**Team:** Girlspower-1 (GPMD) | **Module:** Algorithms, Data Structures, and Connectionist AI

This table shows where each Markdown topic is used in the Study Guide, Test Bank, PPT Slides and Video Tutorials.

**✔** = used in that resource. 

**—** = deliberately not used in that resource (reason in the Notes column).

> Study Guide chapter numbers are taken from the `[Guide §n]` tags in the Test Bank. Slide and video references are filled from the Stage 2 plan and must be confirmed.

## 1. Mapping by Markdown file

| # | Markdown file | Main topics | Study Guide | Test Bank questions | Slides | Video | Notes |
|---|---|---|---|---|---|---|---|
| A1 | `ALGORITHMS/01_Introduction_and_Key_Concepts.md` | Definition, characteristics, pseudocode, conditions, loops | §1 | TF01–03, MC01–02, OE01 | ✔ `<<slide nos.>>` | ✔ `<<video, time>>` | |
| A2 | `ALGORITHMS/02_Searching_and_Sorting_Algorithms.md` (2.2 Searching) | Linear search, binary search | §2 | TF04–07, MC03–05, OE02 | ✔ `<<slide nos.>>` | ✔ `<<video, time>>` | |
| A3 | `ALGORITHMS/02_Searching_and_Sorting_Algorithms.md` (2.3–2.4 Sorting) | Bubble sort, selection sort, choosing an algorithm | §3 | TF08–11, MC06–09, OE03 | ✔ `<<slide nos.>>` | ✔ `<<video, time>>` | Test Bank also asks about insertion sort. See Section 3, item 1 |
| A4 | `ALGORITHMS/03_Algorithm_Efficiency.md` | Big O, time and space complexity, auxiliary space | §4 | TF12–15, MC10–13, OE04 | ✔ `<<slide nos.>>` | ✔ `<<video, time>>` | |
| A5 | `ALGORITHMS/04_Examples_and_Learner_Activities.md` | Worked examples, activities A–E | §1–4 (examples) | OE01–04 | ✔ `<<slide nos.>>` | — | Activities are for self-study. Video covers the worked examples only |
| A6 | `ALGORITHMS/05_Terminology.md` | 20 key terms | Glossary `<<§ or appendix>>` | — | ✔ `<<slide nos.>>` | — | Video explains terms in context, not as a list |
| D1 | `DATA-STRUCTURE/01_Introduction_and_Key_Concepts.md` | Array, linked list, stack, queue, tree, graph; choosing a structure | §5–6 | `<<IDs>>` | ✔ `<<slide nos.>>` | ✔ `<<video, time>>` | |
| D2 | `DATA-STRUCTURE/02_Linear_Data_Structures.md` | Arrays, linked lists, stacks (LIFO), queues (FIFO) | §5 | TF16–20, MC14–19, OE05–06 | ✔ `<<slide nos.>>` | ✔ `<<video, time>>` | |
| D3 | `DATA-STRUCTURE/03_Non_Linear_Data_Structures.md` | Trees, graphs, traversal (BFS/DFS) | §6 | TF21–24, MC20–24, OE07–08 | ✔ `<<slide nos.>>` | ✔ `<<video, time>>` | |
| D4 | `DATA-STRUCTURE/04_Examples_and_Learner_Activities.md` | Python examples, activities 1–7, design challenge | §5–6 | `<<IDs>>` | ✔ `<<slide nos.>>` | ✔ `<<video, time>>` | |
| D5 | `DATA-STRUCTURE/05_Terminology.md` | 18 key terms | Glossary `<<§ or appendix>>` | — | ✔ `<<slide nos.>>` | — | Hash table is defined here only; not taught as a topic |
| C1 | `CONNECTIONIST-AI/01_Introduction_to_Connectionist_AI.md` | What it is, neural networks, applications, advantages and limits, comparison with rule-based systems | §7 | TF25–27, MC25–26, OE09 | ✔ `<<slide nos.>>` | ✔ `<<video, time>>` | |
| C2 | `CONNECTIONIST-AI/02_Basic_Neural_Networks_and_How_They_Learn.md` | Neuron, weight, bias, activation, layers, forward propagation, loss, backpropagation, gradient descent | §7–8 | TF28–30, MC27–30, OE10 | ✔ `<<slide nos.>>` | ✔ `<<video, time>>` | |
| C3 | `CONNECTIONIST-AI/03_Examples_and_Learner_Activities.md` | Prediction worked example, activities A–B | §8 | `<<IDs>>` | ✔ `<<slide nos.>>` | ✔ `<<video, time>>` | |
| C4 | `CONNECTIONIST-AI/04_Terminology.md` | Key terms | Glossary `<<§ or appendix>>` | — | ✔ `<<slide nos.>>` | — | |
| T | `Test bank.md` | 30 true/false, 30 multiple choice, 10 extended response | Chapter tags §1–8 | (itself) | — | — | Self-testing only; not presented in class |

## 2. Test Bank coverage by Study Guide chapter

| Guide § | Topic | Questions | Count |
|---|---|---|---:|
| §1 | What is an algorithm | TF01–03, MC01–02 (+ OE01 with §2) | 5 (+1) |
| §2 | Searching | TF04–07, MC03–05 (+ OE02 with §3) | 7 (+1) |
| §3 | Sorting | TF08–11, MC06–09 (+ OE03 with §4) | 8 (+1) |
| §4 | Efficiency | TF12–15, MC10–13, OE04 | 10 |
| §5 | Linear data structures | TF16–20, MC14–19, OE05–06 | 12 |
| §6 | Non-linear data structures | TF21–24, MC20–24, OE07–08 | 11 |
| §7 | Connectionist AI basics | TF25–27, MC25–26, OE09 | 6 |
| §8 | How neural networks learn | TF28–30, MC27–30 (+ OE10 with §9) | 7 (+1) |
| | **Total** | | **70** |

## 3. Gaps and inconsistencies to resolve before submission

| # | Issue found | Evidence | Fix |
|---|---|---|---|
| 1 | The Test Bank asks about **insertion sort** (TF10, MC with option "Insertion sort", OE03), but the Markdown teaches only bubble and selection sort | `insertion sort` appears in 0 content files and 6 Test Bank lines | Add a short insertion sort section to the content, or reword those questions to bubble/selection sort |
| 2 | **OE10** is tagged `[Guide §8–9]`, but the guide has chapters §1–8 | Test Bank tag | Change to §8, or add the chapter |
| 3 | **Hash tables** are defined in terminology but not taught | D5 terminology | Keep as a defined term only, or add a short section |
| 4 | Stage 2 mapping spelled "MARDOWN", "GPDM" and "neutral network" | Stage 2 report | Corrected in this file |
| 5 | `<<IDs>>` cells for D1, D4 and C3 | | Fill from the Test Bank after checking which questions use those examples |

## 4. Where the resources are located

| Resource | Location |
|---|---|
| Markdown content | CONTENT branch (or `content/` after merging) |
| Visuals | VISUALS branch (or `visuals/` after merging) |
| Study Guide and Test Bank | `<<FILL>>` |
| PPT Slides | `<<FILL: submitted under the Slides assignment, file name>>` |
| Video Tutorials | `<<FILL: submitted under the Video assignment, file names or links>>` |
