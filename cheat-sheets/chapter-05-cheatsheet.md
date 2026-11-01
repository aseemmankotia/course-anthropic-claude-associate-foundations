## Chapter 5 Cheat Sheet: Prompting and Task Execution (14%)

### The 4-Part Prompt Structure
| Component | Purpose | Omission Symptom |
|---|---|---|
| Context | Grounds the model (audience, background, prior output) | Irrelevant or misaligned output |
| Task | States exactly what to do | Off-topic or incomplete output |
| Format | Defines structure (bullets, table, paragraph count) | Wrong structure/length |
| Constraints | Limits (length, tone, exclusions) | Overly verbose/off-tone output |

**Exam rule of thumb:** missing *Format* or *Constraints* is the #1 cause of wrong-length/wrong-style distractor answers.

### Decomposition Decision Rule
- Multiple deliverables with **different formats or audiences** → decompose into sequential prompts.
- Later sections **depend on** earlier output (e.g., recommendations depend on analysis) → run analysis first, feed its output/key points into the next prompt.
- Single deliverable, single format, single audience → one prompt is fine.

### Iterative Refinement vs. Re-Prompting
| Approach | What it does | When to use |
|---|---|---|
| Iterative refinement | Gives specific, targeted feedback on existing output | Output is close but needs adjustment |
| Re-prompting from scratch | Discards prior output and context | Rare — only when the prior approach was fundamentally wrong |

**Exam tip:** correct answers almost always reference or build on the prior output rather than restarting.

### Narrowing an Overly Broad Answer
- Don't retype the original question with more adjectives.
- Don't start a new chat (loses context).
- Do send a specific follow-up: "Focus only on [subset], in [format], under [length]."

### Steering Tone / Length / Format
- **Best method:** provide 1–2 examples (few-shot) of the desired output.
- Repeating instructions like "be formal" without an example is weaker and less consistent across turns.

### Task-Type Strategy Matrix
| Task Type | Strategy |
|---|---|
| Creative | Open-ended framing, minimal constraints, iterate on direction first |
| Analytical | Precise constraints, explicit criteria, structured format, require reasoning |
| Summarization | Explicit length limit, named audience, explicit exclusions |

### Specific Feedback Beats Vague Feedback
- Vague: "make it better" → model guesses, may change unrelated content.
- Specific: "shorten paragraph 2 to 3 sentences, remove jargon" → targeted, fewer iterations.

### Common Exam Traps
1. Choosing a single mega-prompt for a multi-part deliverable with dependent sections (should be decomposed).
2. Picking "start a new chat" or "re-ask from scratch" when iterative refinement is correct.
3. Selecting an answer that omits Format/Constraints as the fix for a length/style problem, or omits Context/Task as the fix for a relevance problem — match the symptom to the missing component.
