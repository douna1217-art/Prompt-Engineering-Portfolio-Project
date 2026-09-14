# Methodology & Evaluation: Market Analysis

## Design Choices
- **Structure (R-T-F Framework):** Segregating Role, Task, and Format ensures professional tone alignment and enforces strict structural compliance for tabular output.
- **Technique (Zero-Shot Chain-of-Thought):** Directing the model through explicit internal reasoning steps before generating final sections reduces superficial bullet points and improves strategic depth.

## Part-by-Part Justification
- `[ROLE]`: Defines executive analytical tone and industry perspective.
- `[CONTEXT] & [TASK]`: Limits domain drift and specifies required input entities.
- `[REASONING PROCESS]`: Prompts multi-stage logical evaluation to prevent generic outputs.
- `[CONSTRAINTS]`: Prevents speculative financial claims and fluff.
- `[FORMAT]`: Enforces clean Markdown tables and distinct section headers.

## Evaluation & Scoring Results

| Metric | Naive Prompt | Designed Prompt (V1) | Designed Prompt (Refined) |
| :--- | :--- | :--- | :--- |
| **Evaluator Score** | 52 / 100 | 84 / 100 | 95 / 100 |

## Comparison & Refinement
- **Naive Output:** Produced generic paragraphs lacking structured comparative data, SWOT analysis, or clear action steps.
- **V1 Designed Output:** Established clear section headers and tables, but strategic recommendations remained too high-level.
- **Refinement Made:** Added explicit internal `[REASONING PROCESS]` instructions and specified precise table column schemas, raising the evaluator score to 95/100.

## Reflection
- **Strengths:** Consistently produces structured executive tables and balanced SWOT breakdowns.
- **Limitations:** Dependent on the quality and detail of user-provided competitor inputs.
- **Next Steps:** Integrate dynamic web-search flags for real-time market data retrieval.
