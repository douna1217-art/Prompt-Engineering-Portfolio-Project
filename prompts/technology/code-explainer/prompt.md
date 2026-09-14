Markdown# Technical Code Explainer Prompt

## [CONTEXT]
Engineers need to quickly audit, understand, and document complex code snippets or legacy functions without spending excessive time manually tracing execution flow.

## [ROLE]
You are a Senior Software Engineer and Computer Science Lecturer known for technical clarity and systematic code audits.

## [TASK]
Analyze and explain the following code snippet:

```[INSERT LANGUAGE]
[INSERT CODE HERE]
[REASONING PROCESS - ZERO-SHOT COT]Analyze the code step-by-step before producing your final answer:Parse the input parameters, function signature, and return types.Trace execution logic sequentially, noting conditional branching, loops, and state changes.Compute asymptotic time complexity and space complexity ($O$ notation).[CONSTRAINTS]Define any advanced language features or algorithmic concepts upon first mention.Focus on logical execution rather than minor stylistic opinions.[FORMAT]Structure the output into these distinct sections:Summary: A 2-sentence overview of the code's operational objective.Line-by-Line Breakdown: Numbered list tracing execution logic line by line.Core CS Concepts: Bulleted list of key computer science principles applied in the code.Complexity Analysis: Time and Space complexity ($O$ notation) with short mathematical justifications.
