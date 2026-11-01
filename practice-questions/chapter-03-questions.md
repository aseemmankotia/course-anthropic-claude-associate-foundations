## Chapter 3: Workflow Integration and Solution Design — Practice Questions

**Q1.** A marketing team wants Claude to draft investor-facing financial summaries pulled from quarterly reports. Which approach BEST balances AI suitability and risk?

A) Let Claude fully own drafting and publishing without any review
B) Avoid using Claude entirely because financial content is too sensitive
C) Use Claude to draft a first version, then have a qualified analyst verify figures and approve before publishing
D) Use Claude only for formatting after a human writes the full content

<details>
<summary>Answer</summary>

**Correct: C**

This is a Hybrid step: Claude accelerates the first draft, but a qualified human validates accuracy and compliance before anything is published.

**Why the others are wrong:**
- Full ownership with no review ignores the human-required accountability needed for investor-facing financial accuracy and compliance.
- Excluding Claude entirely wastes a legitimate optimization opportunity for drafting repetitive structured content.
- Using Claude only for formatting underuses its drafting capability and doesn't reduce the most time-consuming manual work.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q2.** A support team wants to reduce time spent writing repetitive ticket responses. Which workflow design is MOST appropriate?

A) Claude auto-sends replies to all tickets without review
B) Claude drafts suggested replies for agents, who review and send
C) Claude answers FAQ tickets end-to-end with no agent involvement
D) Discontinue Claude use and rely only on canned responses

<details>
<summary>Answer</summary>

**Correct: B**

This Hybrid design captures time savings on repetitive drafting while keeping a human accountable for what actually reaches a customer.

**Why the others are wrong:**
- Sending replies with zero review removes the oversight needed for customer-facing accuracy.
- Even 'FAQ-only' automation can hit edge cases Claude misreads, so some human spot-check remains warranted.
- Dropping Claude entirely discards a clear process-optimization opportunity for repetitive text generation.

</details>

---

**Q3.** A product manager asks Claude to 'find the best competitor pricing strategy and give a definitive answer to present to the board tomorrow.' What is the KEY risk in this request?

A) Claude's output will take too long to generate for a same-day deadline
B) Claude cannot access any information about competitor pricing
C) Claude will refuse the task entirely
D) Treating Claude's exploratory research as a final, verified answer without fact-checking

<details>
<summary>Answer</summary>

**Correct: D**

Asking for a 'definitive' board-ready answer skips the validation step exploratory research requires; the risk is presenting unverified AI output as settled fact.

**Why the others are wrong:**
- Speed is not the limiting factor here — Claude can generate a response quickly, which is part of the risk, not the problem itself.
- Claude can produce plausible pricing analysis from available context; the issue is verification, not access.
- Claude does not categorically refuse general research requests like this.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q4.** A team wants to use Claude to quickly surface ideas and angles for a new feature before committing resources. Which mode of research use is MOST appropriate?

A) Final-answer research — treat Claude's output as the validated source of truth
B) Skip Claude and rely solely on human brainstorming
C) Exploratory research — use Claude to generate options and directions, then validate separately
D) Use Claude to make the final go/no-go investment decision

<details>
<summary>Answer</summary>

**Correct: C**

Early-stage idea generation is exactly where exploratory research adds value — speed and breadth, with human judgment applied before resources are committed.

**Why the others are wrong:**
- Treating early-stage brainstorming output as fully validated truth overstates Claude's role at this exploratory stage.
- Excluding Claude discards a clear speed advantage for divergent idea generation.
- Delegating a resource-commitment decision to Claude overstates its capability and removes human accountability.

</details>

---

**Q5.** An AI orchestrator must classify a workflow step where Claude drafts legal clause language that a licensed attorney must review and approve before use. How should this step be classified?

A) AI-suitable (fully automatable)
B) Hybrid — AI drafts, human validates and approves
C) Human-required (no AI involvement)
D) Unclassifiable because legal work can't use AI at all

<details>
<summary>Answer</summary>

**Correct: B**

Claude contributes drafting value, but final accountability and approval sit with the attorney — the defining pattern of a Hybrid step.

**Why the others are wrong:**
- Fully automatable ignores the mandatory attorney sign-off described in the scenario.
- Human-required with no AI involvement ignores that Claude is explicitly doing the drafting.
- Legal content can use AI assistance as long as a qualified human validates the output — it's not categorically excluded.

</details>

---

**Q6.** A team is designing a workflow for AI-assisted code review. Which configuration BEST reflects proper human-required oversight?

A) Claude flags potential issues and a human reviewer makes the approval/merge decision
B) Claude auto-merges pull requests that pass its own review
C) Claude is excluded from code review entirely due to risk
D) Human reviewers approve all PRs without reading Claude's flagged issues

<details>
<summary>Answer</summary>

**Correct: A**

Claude surfaces candidate issues (AI-suitable work), while the irreversible action — merging — stays with a human decision-maker.

**Why the others are wrong:**
- Letting Claude merge based on its own review removes human accountability from an irreversible action.
- Full exclusion discards the time savings of automated issue flagging.
- Rubber-stamping approvals without reading flags defeats the purpose of the hybrid review step.

</details>

---

**Q7.** When presenting Claude's value to stakeholders, which framing BEST sets realistic expectations without overstating capability?

A) "Claude can accelerate first-draft research and reduce repetitive work, but outputs still require human validation for accuracy."
B) "Claude will replace our research team within the next quarter."
C) "Claude never makes mistakes, so review steps can be eliminated."
D) "Claude's capabilities are unpredictable, so we should avoid using it until it's more mature."

<details>
<summary>Answer</summary>

**Correct: A**

This framing states a concrete benefit (speed on drafts/repetitive work) alongside an explicit, realistic limit (validation still required).

**Why the others are wrong:**
- Claiming full replacement overstates capability and ignores the human-required accountability in most real workflows.
- Claiming Claude never makes mistakes misrepresents its reliability and invites removal of necessary review steps.
- Dismissing Claude as too unpredictable understates its proven value in hybrid, well-scoped workflow steps.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q8.** After integrating Claude into a workflow, a team measures a 40% reduction in time spent on first drafts but notices a slight increase in required review time. What does this illustrate?

A) Claude integration failed and should be reversed
B) The team should remove all review steps to maximize time savings
C) Review time increases always mean Claude's output quality is poor
D) A time-saved vs quality trade-off that should be evaluated holistically, not just by draft speed

<details>
<summary>Answer</summary>

**Correct: D**

Measuring integration success requires weighing total time and quality impact together, not optimizing a single metric like draft speed in isolation.

**Why the others are wrong:**
- A net gain in draft speed with manageable review overhead isn't evidence of failure on its own.
- Removing review steps to chase speed ignores the quality trade-off the scenario is highlighting.
- Slightly more review time doesn't automatically indicate poor quality — it may reflect appropriately thorough validation of faster drafts.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

