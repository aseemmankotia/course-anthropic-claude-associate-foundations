## Chapter 6: Product and Model Selection — Practice Questions

**Q1.** A legal team needs to repeatedly analyze a 150-page contract over several weeks, referencing shared definitions, prior clause analysis, and team-specific instructions each session. Which Claude product BEST meets these requirements?

A) Chat
B) Projects
C) Research mode
D) Artifacts

<details>
<summary>Answer</summary>

**Correct: B**

Projects maintains a persistent knowledge base and custom instructions across many sessions, ideal for ongoing, context-rich work on the same material.

**Why the others are wrong:**
- Chat is session-based and loses context between conversations, forcing the team to re-upload the contract each time.
- Research mode is designed for multi-source exploratory synthesis, not repeated deep analysis of one fixed document.
- Artifacts produces standalone output but doesn't retain persistent shared context across sessions.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q2.** A user wants to quickly rewrite a single paragraph of an email before sending it, with no need to reuse context later. Which product should they use?

A) Projects
B) Research mode
C) Artifacts
D) Chat

<details>
<summary>Answer</summary>

**Correct: D**

Chat is designed for quick, one-off tasks that don't require persistent context or a knowledge base.

**Why the others are wrong:**
- Projects adds unnecessary setup overhead for a single quick edit.
- Research mode is for multi-source exploratory questions, not a one-off rewrite.
- Artifacts is for generating standalone reusable documents, overkill for a single paragraph edit.

</details>

---

**Q3.** A user needs Claude to generate a standalone HTML dashboard they can view, edit, and reuse independently of the chat conversation. Which feature BEST fits this need?

A) Chat
B) Artifacts
C) Projects
D) Research mode

<details>
<summary>Answer</summary>

**Correct: B**

Artifacts renders generated structured content (code, documents, dashboards) in a separate reusable pane distinct from the conversational flow.

**Why the others are wrong:**
- Chat keeps generated content inline within the conversation history only, not as a reusable standalone object.
- Projects manages persistent context across sessions but is not itself the mechanism for generating standalone reusable content.
- Research mode focuses on synthesizing information from multiple sources, not generating structured deliverables.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q4.** An analyst needs Claude to gather and synthesize information from multiple online sources to answer an open-ended, exploratory question with citations. Which capability should they use?

A) Artifacts
B) Chat
C) Research mode
D) Projects

<details>
<summary>Answer</summary>

**Correct: C**

Research mode is purpose-built for multi-source exploratory questions, synthesizing information across sources with citations.

**Why the others are wrong:**
- Artifacts generates standalone content but doesn't perform multi-source research synthesis.
- Chat handles single-turn tasks without the multi-source retrieval and citation behavior of Research mode.
- Projects persists context for recurring work but doesn't inherently perform live multi-source research.

</details>

---

**Q5.** A company processes thousands of simple customer support tickets per hour and needs to classify each into one of five categories as fast and cheaply as possible. Which model is the BEST fit?

A) Opus
B) Haiku
C) Sonnet
D) None — use Research mode instead

<details>
<summary>Answer</summary>

**Correct: B**

Haiku is optimized for fast, low-cost performance on simple, high-volume tasks like classification.

**Why the others are wrong:**
- Opus is the highest-capability, highest-cost model — overkill and too slow/expensive for simple high-volume classification.
- Sonnet is a balanced workhorse but costs more and runs slower than Haiku for this simple repetitive task.
- Research mode is a capability for exploratory multi-source questions, not a model tier, and doesn't apply here.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q6.** A legal team needs Claude to perform nuanced multi-step reasoning over conflicting contract clauses where accuracy matters far more than cost or speed. Which model should they select?

A) Opus
B) Haiku
C) Sonnet
D) Chat

<details>
<summary>Answer</summary>

**Correct: A**

Opus is the highest-capability model, best suited for complex reasoning and nuanced tasks where accuracy outweighs cost or latency concerns.

**Why the others are wrong:**
- Haiku trades capability for speed/cost, making it unsuitable for complex nuanced reasoning.
- Sonnet is the balanced everyday workhorse but is not the top choice when maximum reasoning capability is required.
- Chat is a product/interface, not a model — it doesn't answer the model-selection question being asked.

</details>

---

**Q7.** A user tries to paste an extremely long document that exceeds the model's context window into a single Chat conversation. What is the BEST approach to handle this?

A) Switch to Opus, since it has a larger context window than Sonnet or Haiku
B) Chunk the document into smaller sections or use a Project knowledge base for retrieval instead of pasting it all at once
C) Paste it anyway — Claude will automatically truncate only the irrelevant parts
D) Use Research mode, which has no context window limit

<details>
<summary>Answer</summary>

**Correct: B**

When content exceeds the context window, the correct approach is chunking the document or using a Project's knowledge base for retrieval rather than exceeding the limit in one pass.

**Why the others are wrong:**
- Context window size does not vary meaningfully by model tier in a way that solves this — Haiku, Sonnet, and Opus share the same context window limit.
- Claude does not intelligently auto-truncate to preserve only relevant content; exceeding the limit causes input errors or loss of early content.
- All Claude products, including Research mode, operate within the same underlying context window constraints — there is no mode with unlimited context.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q8.** A marketing associate needs to draft weekly blog posts, summarize meeting notes, and answer routine business questions. Which model is the recommended default choice?

A) Haiku, because cost should always be minimized first
B) Opus, because it is always the safest default
C) Sonnet, as the balanced everyday workhorse for most knowledge-work tasks
D) This task requires Research mode, not a model choice

<details>
<summary>Answer</summary>

**Correct: C**

Sonnet is designed as the balanced default for everyday knowledge-work tasks, offering strong capability without the cost/latency of Opus.

**Why the others are wrong:**
- Minimizing cost at all costs with Haiku risks quality shortfalls on tasks requiring more nuanced writing and reasoning than simple classification.
- Opus is reserved for complex, nuanced reasoning tasks; using it as a default for routine work wastes cost and latency.
- Research mode addresses multi-source exploratory questions, not everyday drafting and summarization — it doesn't replace model selection.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

