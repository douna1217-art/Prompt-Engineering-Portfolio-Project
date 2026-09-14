# Prompt Engineering Frameworks & Reference Guide

## Structural Frameworks

### 1. R-T-F Framework (Role, Task, Format)
- **Role:** Establishes the specific persona, authority, or technical identity the LLM must adopt.
- **Task:** Clear, non-ambiguous functional instruction defining the core operation.
- **Format:** Mandates explicit structural delivery rules (Markdown tables, bullet points, structured JSON).

### 2. C-A-R-E Framework (Context, Action, Result, Example)
- **Context:** Establishes domain parameters, operational environment, and background information.
- **Action:** Step-by-step instructions execution detailing how input data must be processed.
- **Result:** Definite outcome quality expectations, target audience parameters, and tone constraints.
- **Example:** In-context demonstrations guiding format adherence and reasoning style.

---

## Prompting Techniques

| Technique | Definition | Target Application |
| :--- | :--- | :--- |
| **Zero-Shot** | Direct task execution instructions without prior exemplars. | Standard formatting or direct logic generation. |
| **Few-Shot** | Providing 1–3 explicit input/output exemplars within the context window. | Output pattern enforcement, custom formatting, tone alignment. |
| **Chain-of-Thought (CoT)** | Directing the model to output sequential intermediate reasoning steps before final output. | Complex logic, numerical calculation, and multi-step evaluation. |
| **Zero-Shot CoT** | Prompting step-by-step reasoning using explicit execution triggers without providing exemplars. | Algorithmic analysis, logic verification, and rapid problem decomposition. |
