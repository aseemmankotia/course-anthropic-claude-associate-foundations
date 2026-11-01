## Chapter 2: Output Evaluation and Validation — Practice Questions

**Q1.** A company uses Claude to draft a client email summarizing quarterly earnings figures recalled from memory. Which solution BEST addresses the risk of hallucination before sending?

A) Cross-reference every number against the original financial report before sending
B) Ask Claude to double-check its own numbers one more time
C) Reword the email to sound more confident and authoritative
D) Ask Claude to cite the filing by name without checking the figures

<details>
<summary>Answer</summary>

**Correct: A**

Numbers must be traced to the primary source document — this is the only way to catch fabricated or misremembered figures.

**Why the others are wrong:**
- Self-verification checks internal consistency, not ground truth, and is not sufficient evidence for client-facing numbers.
- Tone has no bearing on factual accuracy and can mask errors.
- Naming a source without checking it against the actual data does nothing to validate the figures.

</details>

---

**Q2.** A Claude-generated competitor analysis consistently frames one competitor negatively while leaving out their recent product awards. This is best described as:

A) A hallucination
B) Subtle bias through omission and framing
C) An outdated fact
D) A formatting error

<details>
<summary>Answer</summary>

**Correct: B**

Nothing stated is fabricated or false — the issue is selective emphasis and missing perspective, which is the definition of framing/omission bias.

**Why the others are wrong:**
- Hallucination requires fabricated or non-existent content, not skewed emphasis.
- Outdated implies the information was once accurate but has since changed — not the issue here.
- Formatting refers to structure/layout, not content slant.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q3.** A high-stakes legal brief includes a case citation. When asked to self-verify, Claude confirms the citation is accurate. What should you do next?

A) Trust the self-verification and submit the brief
B) Remove the citation entirely to avoid any risk
C) Independently verify the citation against a legal database
D) Ask Claude to run the same self-verification a second time

<details>
<summary>Answer</summary>

**Correct: C**

Self-verification only tests internal consistency, not whether the citation exists or says what is claimed — high-stakes claims require an external primary-source check.

**Why the others are wrong:**
- Trusting self-verification on high-stakes legal content is the exact trap the exam tests — it is not independent evidence.
- Removing the citation discards potentially valid, useful support rather than validating it.
- Repeating the same self-check does not add new evidence; it will likely return the same unverified answer.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q4.** A manager needs a one-page overview of 15 metrics for quick scanning before a board meeting. Which output format BEST fits this audience need?

A) A structured table grouping the metrics with clear headers
B) Dense narrative prose covering all 15 metrics
C) A single ungrouped bullet list of all 15 items
D) A verbatim transcript of the underlying data pull

<details>
<summary>Answer</summary>

**Correct: A**

A structured table allows rapid comparison and scanning of multiple metrics — the exact need for a time-constrained board audience.

**Why the others are wrong:**
- Prose buries discrete metrics inside sentences, slowing quick scanning.
- An ungrouped list of 15 items has no comparative structure and is harder to scan than a table.
- A raw transcript is unprocessed and not audience-appropriate for a board overview.

</details>

---

**Q5.** Your workflow requires a repeatable fact-check pass on a Claude-generated output. Which sequence correctly matches the required checks?

A) Tone, grammar, formatting
B) Length, keyword density, SEO
C) Claims, numbers, names, dates
D) Self-verification only

<details>
<summary>Answer</summary>

**Correct: C**

A repeatable fact-check pass validates discrete factual claims, numeric values, proper names, and dates independently — these are the categories most prone to silent errors.

**Why the others are wrong:**
- Tone, grammar, and formatting are quality checks, not factual verification.
- Length/keyword/SEO checks are irrelevant to factual accuracy.
- Self-verification alone is not a fact-check workflow — it lacks external confirmation.

</details>

---

**Q6.** Which of the following outputs falls into the tier that REQUIRES mandatory human review before release?

A) An internal brainstorm draft shared with one teammate
B) Personal notes for your own later use
C) An informal internal Slack message draft
D) A client-facing financial recommendation

<details>
<summary>Answer</summary>

**Correct: D**

Client-facing content with financial consequences is high-stakes — mandatory human review is triggered by external audience plus real-world consequence of error.

**Why the others are wrong:**
- Internal brainstorm drafts are low-stakes and reversible, not requiring mandatory review.
- Personal notes have no external audience or consequence.
- Informal internal messages are low-stakes and easily corrected if wrong.

</details>

---

**Q7.** What is the key difference between a hallucination and a factually outdated answer?

A) Hallucinations are always longer than outdated answers
B) A hallucination is fabricated or never-true content; an outdated answer was once true but has since changed
C) Outdated answers are always formatted as bullet points
D) There is no meaningful difference between the two

<details>
<summary>Answer</summary>

**Correct: B**

This distinction determines the correct fix: hallucinations require removal/correction of fabricated content, while outdated answers require refreshing with current data.

**Why the others are wrong:**
- Length has no bearing on whether content is fabricated or outdated.
- Formatting is unrelated to whether a claim is fabricated versus stale.
- Treating them as equivalent leads to misdiagnosing the fix needed — the exam tests this difference directly.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q8.** Claude answers 'What are the risks of this contract?' by listing 3 risks, but the source contract contains 5 distinct risk clauses. This is an example of:

A) A silent omission / completeness failure
B) A hallucination
C) Bias in framing
D) A formatting mismatch

<details>
<summary>Answer</summary>

**Correct: A**

Nothing stated is false, but material content was left out without flagging it — a completeness failure that a dedicated omission check would catch.

**Why the others are wrong:**
- Hallucination requires false or fabricated content, not missing content.
- Bias involves skewed framing of included content, not missing items entirely.
- Formatting mismatch concerns structure/presentation, not missing substantive content.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

