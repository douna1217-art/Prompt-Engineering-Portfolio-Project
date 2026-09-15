# Methodology & Evaluation: Study Guide Generator

## Design Choices
- **Structure (C-A-R-E Framework Variant):** Uses tagged components (`[CONTEXT]`, `[ACTION]`, `[INPUT DATA]`, `[FEW-SHOT EXAMPLES]`, `[RESULT FORMAT]`) to isolate raw notes from structural rules.
- **Technique (Few-Shot Prompting):** Includes an explicit input-output exemplar to condition the AI to output answer keys directly alongside practice items with explanations.

## Part-by-Part Justification
- `[CONTEXT]`: Identifies the educational purpose (generating active-recall study guides from notes).
- `[ACTION]`: Directs the operational transformation process.
- `[INPUT DATA]`: Isolates subject, target academic level, and raw note content.
- `[FEW-SHOT EXAMPLES]`: Demonstrates expected output layout, inline answer keys, and formatting logic.
- `[RESULT FORMAT]`: Mandates Core Concepts Summary, Vocabulary Table, and Practice Quiz.

## Evaluator Scoring Results

| Metric | Naive Prompt | Designed Prompt |
| :--- | :--- | :--- |
| **Clarity & Specificity** | 15 / 30 | 30 / 30 |
| **Structure & Framework Use** | 0 / 30 | 30 / 30 |
| **Context & Inputs** | 10 / 20 | 20 / 20 |
| **Output Requirements** | 0 / 20 | 10 / 20 |
| **TOTAL SCORE** | **25 / 100** | **90 / 100** |

## Comparison & Evaluator Feedback
- **Naive Output Performance (25/100):** Provided raw notes but relied on default assumptions, missing target grade levels, terminology tables, and practice questions.
- **Designed Output Performance (90/100):** Successfully calibrated output depth to high school AP level and enforced inline answer key formatting via few-shot exemplars.
- **Refinement Identified by Gem:** To reach a 100 score, add quantitative item constraints (e.g., specifying the exact number of quiz questions and total word count).

## Reflection
- **Strengths:** Converts unstructured notes into active-recall review materials predictably.
- **Limitations:** Dependability is bound by the factual accuracy of the provided raw user notes.
- **Next Step:** Add explicit parameters for question count (e.g., "Generate exactly 5 multiple choice questions").
