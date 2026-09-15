# Methodology & Evaluation: Market Analysis

## Design Choices
- **Structure (Custom Tagged R-T-F Structure):** Leverages `[ROLE]`, `[TASK]`, `[REASONING PROCESS]`, and `[FORMAT]` to demand strategic industry intelligence instead of basic marketing fluff.
- **Technique (Zero-Shot Chain-of-Thought):** Forces internal market trend analysis and competitor benchmarking prior to generating tables and recommendations.

## Part-by-Part Justification
- `[ROLE]`: Establishes the authoritative perspective of a Senior Strategic Market Analyst.
- `[TASK]`: Bounds the target product, exact demographic age group (18–24), and direct competitors.
- `[REASONING PROCESS]`: Directs the AI to evaluate macro trends and isolate positioning drivers before writing.
- `[FORMAT]`: Enforces Executive Summary, Competitor Comparison Table, SWOT Analysis, and Action Steps.

## Evaluator Scoring Results

| Metric | Naive Prompt | Designed Prompt |
| :--- | :--- | :--- |
| **Clarity & Specificity** | 15 / 30 | 30 / 30 |
| **Structure & Framework Use** | 0 / 30 | 30 / 30 |
| **Context & Inputs** | 0 / 20 | 20 / 20 |
| **Output Requirements** | 0 / 20 | 10 / 20 |
| **TOTAL SCORE** | **15 / 100** | **90 / 100** |

## Comparison & Evaluator Feedback
- **Naive Output Performance (15/100):** Returned generic business prose missing target demographic bounds, competitor tables, and SWOT breakdowns.
- **Designed Output Performance (90/100):** Successfully generated structured comparative tables, SWOT metrics, and targeted strategic advice for the specified age demographic.
- **Refinement Identified by Gem:** To reach a perfect score, include explicit word-count or section length boundaries in the format constraints.

## Reflection
- **Strengths:** Guarantees actionable strategy outputs with standardized Markdown comparative tables.
- **Limitations:** Requires accurate listing of primary industry rivals in the input parameters.
- **Next Step:** Add strict length boundaries (e.g., "Limit Executive Summary to 150 words").
