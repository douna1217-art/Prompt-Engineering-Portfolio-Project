# Methodology & Evaluation: Code Explainer

## Design Choices
- **Structure (Custom Context-Role-Task-Reasoning-Format):** Enforces a pedagogical sequence that moves from high-level summary down to line-by-line execution and formal algorithmic complexity analysis.
- **Technique (Zero-Shot Chain-of-Thought):** Requiring the model to explicitly execute internal logical tracing before writing explanations eliminates syntax misinterpretations and hallucinated variable states.

## Part-by-Part Justification
- `[CONTEXT] & [ROLE]`: Establishes precise educational authority and technical rigor.
- `[REASONING PROCESS]`: Forces internal line-by-line execution tracing prior to output compilation.
- `[CONSTRAINTS]`: Ensures jargon is explained and prevents generic stylistic commentary.
- `[FORMAT]`: Mandates clean Markdown sections and mathematical LaTeX formatting for Big-O metrics.

## Evaluation & Scoring Results

| Metric | Naive Prompt | Designed Prompt (V1) | Designed Prompt (Refined) |
| :--- | :--- | :--- | :--- |
| **Evaluator Score** | 58 / 100 | 88 / 100 | 96 / 100 |

## Comparison & Refinement
- **Naive Output:** Returned a single-sentence overview without tracing logic, explaining data structures, or evaluating complexity.
- **V1 Designed Output:** Provided line breakdowns and summaries, but missed formal Big-O space complexity calculations.
- **Refinement Made:** Explicitly requested both time and space complexity ($O$ notation) with mathematical justifications in `[REASONING PROCESS]` and `[FORMAT]`, raising the score to 96/100.

## Reflection
- **Strengths:** Excellent for technical documentation, code reviews, and onboarding.
- **Limitations:** Large codebases (>500 lines) should be decomposed into modular functions prior to analysis.
- **Next Steps:** Add an optional code optimization/refactoring output block.
