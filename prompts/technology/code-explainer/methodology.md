# Methodology & Evaluation: Code Explainer

## Design Choices
- **Structure (Custom Tagged Structure):** Segregates `[CONTEXT]`, `[ROLE]`, `[TASK]`, `[REASONING PROCESS]`, and `[FORMAT]` to enforce technical depth and a professional pedagogy.
- **Technique (Zero-Shot Chain-of-Thought):** Enforces explicit step-by-step code execution tracing and asymptotic complexity calculation ($O$ notation) prior to output generation.

## Part-by-Part Justification
- `[CONTEXT]`: Identifies the practical operational requirement (auditing legacy code snippets).
- `[ROLE]`: Establishes an authoritative persona (Senior Software Engineer / Lecturer).
- `[TASK]`: Bounds the core objective and provides the typed code block.
- `[REASONING PROCESS]`: Prompts explicit intermediate execution tracing and Big-O evaluation.
- `[FORMAT]`: Specifies clean output sections (Summary, Line Breakdown, CS Concepts, Complexity Analysis).

## Evaluator Scoring Results

| Metric | Naive Prompt | Designed Prompt |
| :--- | :--- | :--- |
| **Clarity & Specificity** | 15 / 30 | 30 / 30 |
| **Structure & Framework Use** | 0 / 30 | 30 / 30 |
| **Context & Inputs** | 0 / 20 | 20 / 20 |
| **Output Requirements** | 0 / 20 | 10 / 20 |
| **TOTAL SCORE** | **15 / 100** | **90 / 100** |

## Comparison & Evaluator Feedback
- **Naive Output Performance (15/100):** Returned a basic, unconstrained functional description without structural breakdown, technical context, or complexity analysis.
- **Designed Output Performance (90/100):** Successfully triggered zero-shot step-by-step reasoning, produced clean line-by-line tracing, and calculated asymptotic time/space complexity.
- **Refinement Identified by Gem:** To reach a perfect 100 score, specify explicit length or word-count boundaries (e.g., maximum word counts or conciseness limits) inside the output constraints.

## Reflection
- **Strengths:** Eliminates high-level generic summaries by forcing line-by-line technical execution tracing.
- **Limitations:** Focuses on single function snippets; large codebases require modular breakdown before processing.
- **Next Step:** Add explicit word-count bounds and optional refactoring recommendations.
