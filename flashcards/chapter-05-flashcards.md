## Chapter 5: Prompting and Task Execution — Flashcards

| # | Front (Question) | Back (Answer) |
|---|-----------------|---------------|
| 1 | Four components of a well-structured prompt? | Context, Task, Format, Constraints. Exam tip: missing Format or Constraints is the most common cause of wrong-length or wrong-style output on exam scenarios. |
| 2 | Report needs analysis + recommendations — one prompt or decomposed? | Decompose: Prompt 1 = analysis, Prompt 2 = recommendations built on that analysis output. Exam tip: dependent multi-part deliverables should be sequenced, not combined. |
| 3 | Iterative refinement vs. re-asking from scratch — which is preferred? | Iterative refinement: give specific feedback on the existing output. Re-asking discards useful context and wastes turns. Exam tip: correct answers reference the prior output. |
| 4 | Most reliable way to steer tone, length, or format? | Provide one or two examples (few-shot) matching the desired output. Exam tip: showing beats repeated telling for style-sensitive tasks. |
| 5 | Prompting strategy for creative tasks? | Open-ended framing, minimal rigid constraints, iterate on direction before polishing. Exam tip: over-constraining creative tasks early reduces output quality. |
| 6 | Prompting strategy for analytical tasks? | Precise constraints, explicit evaluation criteria, structured output (e.g., table), request supporting reasoning. Exam tip: ambiguity is the main failure mode for analytical prompts. |
| 7 | Prompting strategy for summarization tasks? | Specify length, target audience, and what to exclude. Exam tip: without an explicit length constraint, summaries default to overly long. |
| 8 | First response is too broad — best next move? | Send a narrowing follow-up (e.g., 'focus only on X' or 'go deeper on Y') instead of rewriting the original prompt. Exam tip: narrowing follow-ups preserve context and save turns. |
| 9 | Sign that a task is too much for a single prompt? | It bundles multiple distinct deliverables with different formats/audiences (e.g., 'write code, test it, document it, and summarize for execs'). Exam tip: distinct formats/audiences = decompose. |
| 10 | 'Make it better' vs 'Shorten paragraph 2 to 3 sentences and remove jargon' — which is better feedback? | The specific, actionable feedback. Vague feedback forces the model to guess and often changes unrelated parts. Exam tip: specificity reduces the number of iterations needed. |
| 11 | Constraints component of a prompt — typical examples? | Word/length limits, tone, output format (bullets vs. prose), exclusions, audience level. Exam tip: constraints are the most frequently omitted component in exam distractor answers. |
| 12 | When decomposing a report task, what belongs in Prompt 2? | A brief restatement of key facts/output from Prompt 1, plus the new task instruction. Exam tip: don't assume perfect memory of long prior outputs — restate key points if needed. |
