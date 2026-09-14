# Study Guide & Assessment Generator Prompt

## [CONTEXT]
Students require structured study guides that convert raw lecture notes or textbook excerpts into key takeaways, defined terminology tables, and active-recall practice questions.

## [ACTION]
Transform the provided raw lecture notes into an organized study guide accompanied by a self-assessment quiz.

## [INPUT DATA]
- **Subject:** [INSERT SUBJECT]
- **Target Academic Level:** [INSERT LEVEL e.g., High School AP, Undergraduate]
- **Raw Notes:**
## [FEW-SHOT EXAMPLES]

### Example Input:
Subject: Biology
Level: High School
Notes: Photosynthesis light reactions happen in thylakoids making ATP. Calvin cycle happens in stroma using ATP to make glucose.

### Example Output:

#### 1. Core Concepts Summary
- **Light-Dependent Reactions:** Occur within thylakoid membranes; convert light energy into chemical energy (ATP and NADPH).
- **Calvin Cycle (Light-Independent):** Takes place in the stroma; uses stored ATP and NADPH to fix carbon into glucose.

#### 2. Key Terminology Table
| Term | Definition |
| :--- | :--- |
| **Thylakoid** | Membrane-bound compartment inside chloroplasts where light reactions occur. |
| **Stroma** | Fluid-filled space surrounding thylakoids where carbon fixation takes place. |

#### 3. Practice Quiz
1. Where do light-independent reactions take place?
   - A) Thylakoid membrane
   - B) Stroma
   - C) Mitochondria
   *Answer: B — The Calvin cycle occurs in the stroma.*

---

## [RESULT FORMAT]
Structure the final output as follows:
1. **Core Concepts Summary**: Bulleted breakdown of primary themes.
2. **Key Terminology Table**: Markdown table with `Term` and `Definition` columns.
3. **Practice Quiz**: 3 Multiple-Choice Questions and 2 Short Answer Questions, each complete with an explicit answer key and explanatory rationale.
