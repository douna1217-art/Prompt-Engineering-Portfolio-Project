# Methodology & Evaluation: Study Guide Generator

## Design Choices
- **Structure (C-A-R-E Framework):** Segregating Context, Action, Result parameters, and Examples ensures clear operational separation between instructions and input data.
- **Technique (Few-Shot Prompting):** Providing a concrete worked example within the prompt conditions the model to output answer keys directly underneath quiz items rather than appending them at the end.

## Part-by-Part Justification
- `[CONTEXT] & [ACTION]`: Focuses generation on active-recall pedagogical strategies.
- `[INPUT DATA]`: Isolates user notes to prevent data contamination with general instructions.
- `[FEW-SHOT EXAMPLES]`: Enforces exact formatting standards for quiz questions and explanations.
- `[RESULT FORMAT]`: Ensures consistent structural presentation across subjects.

## Evaluation & Scoring Results

| Metric | Naive Prompt | Designed Prompt (V1) | Designed Prompt (Refined) |
| :--- | :--- | :--- | :--- |
| **Evaluator Score** | 50 / 100 | 85 / 100 | 95 / 100 |

## Comparison & Refinement
- **Naive Output:** Returned a brief summary bullet list missing vocabulary tables, practice questions, or answer rationale.
- **V1 Designed Output:** Generated study guides and quiz items, but question answer keys were omitted.
- **Refinement Made:** Added explicit Few-Shot exemplars demonstrating answer rationale placement, boosting the score to 95/100.

## Reflection
- **Strengths:** Converts messy notes into structured active-recall study sheets instantly.
- **Limitations:** Dependent on the factual completeness of provided source notes.
- **Next Steps:** Add flashcard formatting compatible with spaced-repetition software (Anki).
