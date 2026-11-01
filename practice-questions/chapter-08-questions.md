## Chapter 8: Troubleshooting and Optimization — Practice Questions

**Q1.** A user repeatedly rewrites prompts for a marketing summary but keeps getting generic, vague copy. What is the most effective diagnostic step before trying another prompt variation?

A) Switch to a larger or more capable model
B) Add more exclamation points and urgency to the prompt
C) Lower the temperature setting to reduce randomness
D) Ask Claude what additional context or detail it would need to produce a stronger response

<details>
<summary>Answer</summary>

**Correct: D**

Using Claude's own feedback to surface what's missing directly targets the likely root cause: missing context or ambiguous instructions.

**Why the others are wrong:**
- Model capability is rarely the cause of generic output when the prompt itself lacks specificity.
- Stylistic emphasis does not address missing context or unclear instructions.
- Temperature affects randomness/creativity, not whether the prompt supplied enough context.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q2.** A user needs Claude to reference the same 15-page style guide consistently across dozens of unrelated chat sessions without retyping it each time. Which approach best solves this?

A) Add the style guide to a Project's knowledge base
B) Paste the style guide into the first message of every new chat
C) Reduce the maximum response length in settings
D) Switch to a completely different AI model

<details>
<summary>Answer</summary>

**Correct: A**

Project knowledge sources persist across sessions, which is exactly the recurring-context problem described.

**Why the others are wrong:**
- Re-pasting is tedious and doesn't solve the recurrence problem at a systemic level.
- Response length is unrelated to context persistence.
- The issue is architecture/workflow, not model choice.

</details>

---

**Q3.** Over several weeks, every response from Claude includes unwanted preamble like 'Sure! Here's...' before the actual content. What is the best configuration-level fix?

A) Manually delete the preamble from each response after it's generated
B) Ask Claude to be more concise within each individual prompt, every time
C) Add a custom instruction stating responses should contain only the requested content with no preamble
D) Switch to the API exclusively to avoid formatting issues

<details>
<summary>Answer</summary>

**Correct: C**

A recurring problem across sessions should be fixed at the custom instruction level, not re-solved prompt by prompt.

**Why the others are wrong:**
- Manual deletion doesn't scale and must be repeated indefinitely.
- Repeating the fix in each prompt treats a systemic issue as a one-off, wasting effort.
- Switching surfaces is unnecessary when a simple custom instruction solves the problem.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q4.** What is the primary diagnostic question an operator should ask when a Claude output is weak?

A) Is the model too small for this task?
B) Should I just regenerate the response and hope for better luck?
C) What did I actually ask for versus what did I actually want?
D) Is there an outage affecting the service?

<details>
<summary>Answer</summary>

**Correct: C**

Comparing the literal request to the intended outcome reveals the gap caused by missing context, ambiguity, or format issues.

**Why the others are wrong:**
- Jumping to model capability skips the more likely cause: prompt clarity.
- Regenerating without changes doesn't diagnose or fix the root cause.
- Service outages are an infrastructure concern, not a prompt quality issue.

</details>

---

**Q5.** A team's deployed onboarding workflow uses 12 manual steps, including three separate prompts solely to reformat output between steps. The workflow still produces correct results. What is the appropriate optimization action?

A) Leave the workflow unchanged since it already produces correct output
B) Replace Claude entirely with a different tool
C) Add additional validation steps to increase reliability
D) Consolidate the redundant reformatting steps and tighten the format request in the original prompt

<details>
<summary>Answer</summary>

**Correct: D**

Post-deployment optimization means trimming redundant steps and tightening format requests, even when the workflow technically works.

**Why the others are wrong:**
- 'It works' is not the same as 'it's optimized' — the exam tests proactive workflow improvement.
- Switching tools is an extreme, unnecessary response to a fixable prompt/workflow issue.
- Adding more steps increases complexity, which is the opposite of the optimization goal.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q6.** A user asks Claude to 'write something about our Q3 performance' and receives a vague, generic summary. What is the most likely root cause?

A) Claude lacks sufficient general knowledge about financial performance topics
B) The context window is too small to process the request
C) The temperature setting is too high
D) The instruction is ambiguous and omits context such as audience, data source, and desired format

<details>
<summary>Answer</summary>

**Correct: D**

This matches the core root causes: missing context and ambiguous instructions, not a knowledge or capability gap.

**Why the others are wrong:**
- Claude has broad general knowledge of financial reporting concepts; the issue is prompt specificity, not knowledge.
- Context window limits apply to document length, not a short vague request like this.
- Temperature affects creativity/randomness, not whether required details were supplied.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q7.** Claude responds to a request with: 'Could you clarify whether you want a bulleted list or a narrative paragraph?' What should the operator do?

A) Treat it as a diagnostic signal revealing an ambiguous format request, then update the prompt accordingly
B) Ignore it and resend the identical original prompt
C) Immediately switch to a different AI tool
D) Assume the model is malfunctioning and file a bug report

<details>
<summary>Answer</summary>

**Correct: A**

Clarifying questions from Claude directly reveal which part of the prompt was underspecified; they should be used as free diagnostic feedback.

**Why the others are wrong:**
- Resending the identical prompt ignores useful diagnostic information and wastes a turn.
- Switching tools is unnecessary for a simple format ambiguity.
- A clarifying question is expected, helpful behavior, not a malfunction.

</details>

---

**Q8.** A user consistently needs Claude to execute multi-step coding tasks requiring file system access and terminal commands, but is only using the Claude.ai chat interface and keeps getting stuck. What is the most likely fix?

A) Rewrite the chat prompt with more detailed instructions
B) Lower the temperature setting in the chat interface
C) Switch to Claude Code, which is designed for agentic coding tasks with file and terminal access
D) Add more custom instructions to the Claude.ai chat settings

<details>
<summary>Answer</summary>

**Correct: C**

This is a surface/capability mismatch, not a prompt quality issue — Claude.ai chat does not provide file system or terminal access, while Claude Code does.

**Why the others are wrong:**
- No amount of prompt rewriting grants the chat interface actual file or terminal execution capability.
- Temperature does not affect available tool/execution capabilities.
- Custom instructions cannot grant a surface capabilities it does not support.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

