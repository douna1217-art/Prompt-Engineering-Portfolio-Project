# Prompt Engineering Frameworks & Reference Guide

## Prompt Structural Frameworks

### 1. R-T-F Framework (Role, Task, Format)
- **Role:** Specifies the identity, persona, or domain expertise the LLM should adopt.
- **Task:** Clear, actionable instruction detailing what the LLM must accomplish.
- **Format:** Dictates output structure (e.g., bulleted lists, Markdown tables, executive summaries).

### 2. C-A-R-E Framework (Context, Action, Result, Example)
- **Context:** Provides background information and operational domain constraints.
- **Action:** Detailed functional instructions for processing the input.
- **Result:** Specifies expected output quality, tone, and delivery style.
- **Example:** Demonstrative input/output pairs guiding model execution.

---

## Prompting Techniques

| Technique | Definition | Optimal Use Case |
| :--- | :--- | :--- |
| **Zero-Shot** | Direct instruction without providing explicit examples. | Simple, straightforward generation tasks. |
| **Few-Shot** | Includes one or more worked input/output examples. | Formatting enforcement and custom output styling. |
| **Chain-of-Thought (CoT)** | Explicitly prompts step-by-step internal reasoning. | Complex logic, code analysis, and multi-step decisions. |**
