# Prompt Methodology & Evaluation

## Design Choices

### Structure: R-T-F Framework (Role, Task, Format)
- **Role**: Setting the persona as a "senior strategic marketing analyst" establishes an executive, authoritative tone.
- **Task**: Explicitly directs the model to perform a multi-angle analysis rather than returning generic marketing copy.
- **Constraints**: Prevents fluff and keeps recommendations grounded in actionable business strategy.

### Technique: Zero-shot Chain-of-Thought
- **Reasoning**: Market analysis requires logical deduction. Adding the instruction *"Think through demographic trends, pain points, and competitive advantage step-by-step"* forces the model to deliberate before outputting recommendations, reducing hallucinations.

---

## Evaluation & Scoring (AI Evaluator Results)

| Metric | Naive Prompt | Designed Prompt |
| :--- | :--- | :--- |
| **Prompt Score** | **58 / 100** | **94 / 100** |
| **Structure Clarity** | Low (Single sentence) | High (Labeled sections) |
| **Output Consistency** | Unpredictable format | Standardized 4-part report |

### Gem Evaluator Feedback Comparison
- **Naive Prompt**: *"Write a market analysis for a solar-powered backpack."*
  - *Result*: Generated generic bullet points without market segmentation, channel strategies, or clear tone consistency.
- **Designed Prompt**: 
  - *Result*: Provided structured insights, identified clear pain points (e.g., off-grid charging needs for hikers), and generated concrete channel strategies.
