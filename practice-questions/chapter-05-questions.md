## Chapter 5: Prompting and Task Execution — Practice Questions

**Q1.** A user needs a document with an executive summary, detailed analysis, and recommendations. Which approach BEST meets this requirement?

A) Decompose into sequential prompts: analysis first, then recommendations built on that analysis, then a summary of both
B) Ask for all three sections in one prompt with detailed formatting instructions
C) Ask the model to write the whole report, then say 'make it better' if unsatisfied
D) Write the entire report using one highly detailed system prompt with no follow-up turns

<details>
<summary>Answer</summary>

**Correct: A**

Sequencing lets each section use the output of the prior step as grounded context, which is critical for dependent content like recommendations that must flow from the analysis.

**Why the others are wrong:**
- A single mega-prompt increases the chance that one section's requirements get under-addressed or blended incorrectly
- Vague feedback like 'make it better' gives the model no specific target to fix
- No iteration means no chance to catch dependency errors (e.g., recommendations not matching the analysis) before finalizing

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q2.** Which prompting style BEST fits an open-ended creative brainstorming task?

A) Open-ended framing with minimal constraints, refined through iteration
B) Rigid structured constraints with a strict word count and required format
C) A single highly detailed prompt specifying every plot point upfront
D) A prompt that only lists exclusions with no positive direction

<details>
<summary>Answer</summary>

**Correct: A**

Creative tasks benefit from exploration space before narrowing; heavy constraints early suppress generative variety.

**Why the others are wrong:**
- Excessive structure upfront limits the model's creative range
- Specifying every detail removes the model's generative contribution, defeating the purpose of brainstorming
- Exclusions alone give no positive direction for what to generate

</details>

---

**Q3.** A prompt produces an output of the wrong length and style. Which missing prompt component is the MOST likely cause?

A) Context
B) Task
C) A worked example
D) Format/Constraints

<details>
<summary>Answer</summary>

**Correct: D**

Format and constraints directly dictate length, style, and structure; omitting them leaves the model to default assumptions that rarely match intent.

**Why the others are wrong:**
- Missing context mainly affects accuracy or relevance, not length/style
- Missing task leads to off-topic output, not a length/style mismatch
- Examples help steer style but are not one of the four core structural components (context, task, format, constraints)

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q4.** The model returns a broad, lengthy answer to 'Explain cloud security.' What is the BEST next step?

A) Re-type the original question with more adjectives
B) Start a brand-new chat session and ask the same question again
C) Send a narrowing follow-up such as 'Focus only on identity and access management, in 3 bullet points'
D) Reply only with 'fix it'

<details>
<summary>Answer</summary>

**Correct: C**

A narrowing follow-up uses existing context and specifies the exact subset and format desired, which is faster than restarting or giving vague feedback.

**Why the others are wrong:**
- Adding adjectives doesn't change scope, so the same breadth likely recurs
- Starting over loses the conversational context already built up, wasting a turn
- 'Fix it' is too vague to produce a targeted change

</details>

---

**Q5.** What distinguishes iterative refinement from re-prompting from scratch?

A) Iterative refinement always uses fewer tokens
B) Re-prompting from scratch is always faster
C) There is no meaningful difference between the two approaches
D) Iterative refinement gives specific feedback on the existing output to improve it, while re-prompting discards the prior output and context

<details>
<summary>Answer</summary>

**Correct: D**

This is the core definitional distinction: refinement builds on existing output, re-prompting starts over.

**Why the others are wrong:**
- Token usage depends on the feedback given, not guaranteed to be lower
- Re-prompting often requires re-establishing context, which can be slower overall
- The two approaches produce meaningfully different outcomes and efficiency

</details>

---

**Q6.** Which technique MOST reliably controls output tone (e.g., formal vs. casual) across multiple turns?

A) Repeating 'be formal' in every single message
B) Providing one or two examples of the desired tone early in the conversation
C) Increasing the length of the task description
D) Letting the model guess the appropriate tone

<details>
<summary>Answer</summary>

**Correct: B**

Examples (few-shot) anchor tone more reliably than repeated instructions because the model pattern-matches directly against demonstrated style.

**Why the others are wrong:**
- Repeated instructions without examples are often diluted or inconsistently applied across turns
- A longer task description doesn't inherently define tone
- Guessing introduces inconsistency with no anchor to follow

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q7.** A user needs a one-paragraph summary of a 50-page report for executives. Which prompt is BEST structured?

A) 'Summarize this report.'
B) 'Summarize this report in as much detail as possible.'
C) 'Summarize this report in exactly one paragraph (under 100 words), written for a non-technical executive audience, focusing on financial impact and excluding methodology details.'
D) 'Give me the key points, however many are needed.'

<details>
<summary>Answer</summary>

**Correct: C**

It includes task, format/length constraint, audience context, and an explicit exclusion — all four core prompt components.

**Why the others are wrong:**
- Missing format, length, and audience leads to inconsistent, likely overlong output
- Directly contradicts the need for a brief, one-paragraph summary
- Open-ended length defeats the one-paragraph requirement

</details>

---

**Q8.** When decomposing a multi-part task into sequential prompts, what should typically be included in the second prompt?

A) A brief restatement of key output/facts from the first prompt plus the new task instruction
B) Nothing from the first prompt — treat it as fully independent
C) Only the original system prompt repeated verbatim
D) A request to redo the first prompt's task along with the new one

<details>
<summary>Answer</summary>

**Correct: A**

Carrying forward key facts or output grounds the next step and prevents the model from losing or incorrectly re-deriving earlier context.

**Why the others are wrong:**
- Full independence risks inconsistency between the sequential parts
- Repeating only the system prompt doesn't supply the actual content needed for continuity
- Redoing the first task wastes effort and risks producing a different, inconsistent result

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

