# Development Status and Task Plan

**Last updated:** `<<FILL: date>>` | **Current stage:** Stage 3: Final Markdown Content and Repository (due 28 November 2026, 23:59 Beijing time)


## 1. Project Timeline

| Stage | Focus | Status |
|---|---|---|
| Stage 1 | Planning and content foundation: repository, branches, outline, planning documents | Completed |
| Stage 2 | First versions of the Study Guide and Test Bank, PPT Slides and Video Tutorials; live mini lecture | Completed 
|
| Stage 3 | Finalize the Markdown content, check consistency across all resources, organize the repository, verify and submit | In progress |

## 2. Deliverables

| Deliverable | Description | Status | Location |
|---|---|---|---|
| Markdown learning content | 14 files across Algorithms, Data Structures and Connectionist AI | Final / In review | CONTENT branch |
| Visuals | Diagrams and illustrations | Final / In review | VISUALS branch |
| Study Guide and Test Bank | 8 chapters and a 70-question test bank |  | See [DELIVERABLES.md](../DELIVERABLES.md) |
| PPT Slides | 1 slide deck |  | See [DELIVERABLES.md](../DELIVERABLES.md) |
| Video Tutorials | 4 videos |  | See [DELIVERABLES.md](../DELIVERABLES.md) |
| Resource mapping | Markdown topic to guide, test bank, slides and videos |  | `07_Resource_Mapping.md` |
| Final Submission Report | Revision summary, repository evidence, contributions, verification |  | Submission package |

## 3. Task Plan

| # | Task | Expected result | Owner | Status |
|---|---|---|---|---|
| 1 | Prepare the project outline and learning objectives | Planning documents 01 and 02 | `<<>>` | Completed |
| 2 | Identify prerequisite knowledge | `03_Prerequisite_Knowledge.md` | `<<>>` | Completed |
| 3 | Plan examples and learner activities | `04_Planned_Examples_and_Learner_Activities.md` | `<<>>` | Completed |
| 4 | Write the Markdown content for the three topics | Content files in the CONTENT branch | `<<>>` | Completed |
| 5 | Create visuals | Files in the VISUALS branch | `<<>>` | Completed |
| 6 | Collect and organize references | `06_References_and_Resources.md` | `<<>>` | `<<confirm>>` |
| 7 | Produce the Study Guide and Test Bank | One Study Guide with Test Bank | `<<>>` | Completed `<<confirm>>` |
| 8 | Produce the PPT Slides | One slide deck | `<<>>` | Completed `<<confirm>>` |
| 9 | Produce the Video Tutorials | Four videos | `<<>>` | Completed `<<confirm>>` |
| 10 | Deliver the live mini lecture and record audience questions | Notes on feedback and questions | `<<>>` | Completed `<<confirm>>` |
| 11 | Review and revise content using teacher, peer and mini lecture feedback | Revised content and Final Revision Summary | `<<>>` | In progress |
| 12 | Check consistency across Markdown, guide, test bank, slides and videos | Updated resource mapping; no contradictions | `<<>>` | In progress |
| 13 | Organize the repository and update the README | Clear structure, README, clean file names | `<<>>` | In progress |
| 14 | Final verification | Checklist completed in the report | `<<>>` | Not started |
| 15 | Prepare and submit the package | ZIP with source snapshot, PDF and report | `<<>>` | Not started |

## 4. Open Issues

These problems were found during review and must be resolved or explained before submission.

| # | Issue | Where | Planned fix | Owner | Status |
|---|---|---|---|---|---|
| 1 | The Test Bank asks about insertion sort, but the content teaches only bubble and selection sort | Test Bank (TF10, a multiple-choice item, OE03); Algorithms file 02 | Add an insertion sort section, or reword the questions | `<<>>` | Open |
| 2 | OE10 is tagged `[Guide §8–9]`, but the guide has chapters 1 to 8 | Test Bank | Correct the tag | `<<>>` | Open |
| 3 | The CONTENT README links to folders and files that do not exist | CONTENT README | Delete it or correct the links | `<<>>` | Open |
| 4 | File name errors: `.md.md`, `neutral`, terminology numbering, spaces in names | CONTENT and VISUALS | Rename with `git mv`; update links | `<<>>` | Open |
| 5 | Content files do not embed the visuals | Content files | Add images with relative paths | `<<>>` | Open |
| 6 | Connectionist AI files 01 and 02 repeat explanations of neurons, weights, loss and backpropagation | CONNECTIONIST-AI | Remove repetition; keep one clear explanation | `<<>>` | Open |
| 7 | No single module overview or prerequisites page in the content | CONTENT | Add a short overview | `<<>>` | Open |
| 8 | Hash tables are defined in terminology but not taught | Data Structures terminology | Keep as a defined term only, or add a short section | `<<>>` | Open |

Mark an issue **Resolved** only after a second member has checked the fix, and note the commit ID.

## 5. Final Checks Before 28 November 2026

- [ ] All core topics contain finished, checked content with no placeholders
- [ ] Definitions, examples and answers agree across all resources
- [ ] Open issues above are resolved or explained in the report
- [ ] README and resource mapping are up to date
- [ ] Rendered PDF matches the Markdown source
- [ ] Repository commit matches the submitted snapshot
- [ ] ZIP extracted into a different folder and opened successfully
- [ ] All members have reviewed the final submission

## 6. Updating This Document

Update task statuses as work progresses. When a task is delayed, record the reason and any change of owner or deadline. Keep earlier versions available in the Git history rather than creating copies.
