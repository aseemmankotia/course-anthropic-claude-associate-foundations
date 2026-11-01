## Chapter 4: Governance, Risk, and Responsible Use — Practice Questions

**Q1.** An HR analyst wants to paste a spreadsheet of employee performance reviews — including names, salaries, and SSNs — into Claude to generate summary statistics. What is the BEST course of action?

A) Paste the data as-is since Claude does not store conversation data permanently
B) Remove or mask names, SSNs, and salary figures before pasting, keeping only the data needed for the summary
C) Use a personal Claude account instead of the corporate one to avoid policy review
D) Convert the spreadsheet to a PDF first, then paste it since file uploads are treated differently than text

<details>
<summary>Answer</summary>

**Correct: B**

Redacting direct identifiers (SSNs, names) and sensitive fields (salary) before sharing content with an AI tool is the standard data-minimization practice required before pasting restricted/PII data into any prompt.

**Why the others are wrong:**
- Claude's data handling policy does not eliminate the organization's obligation to avoid exposing PII in the first place — the risk exists the moment it's typed into the prompt.
- Switching accounts to avoid policy review is a governance violation, not a technical fix, and doesn't address the underlying PII exposure.
- File format does not change the sensitivity classification of the data or the need for redaction.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q2.** A marketing team asks Claude to generate customer testimonials that will be published as if real customers wrote them, without disclosing AI involvement. Which inappropriate-use category does this fall into?

A) Unauthorized data sharing
B) Regulated decision-making
C) Deceptive content
D) Data sensitivity violation

<details>
<summary>Answer</summary>

**Correct: C**

Presenting AI-generated content as authentic human testimony without disclosure misleads the audience, which is the definition of deceptive content — a core inappropriate-use category.

**Why the others are wrong:**
- No external data is being shared here; the issue is the output's truthfulness, not data handling.
- No regulated decision (credit, employment, medical, legal) is being made in this scenario.
- No sensitive data classification is involved — the concern is fabricated authenticity, not confidentiality.

</details>

---

**Q3.** A hiring manager wants to use Claude's resume ranking output as the sole and final basis for rejecting candidates, with no human review. Why is this an inappropriate use case?

A) Claude cannot process resumes in bulk
B) It violates data-sensitivity rules because resumes contain PII
C) It constitutes a regulated/high-stakes automated decision made without required human oversight
D) Claude's output format is incompatible with applicant tracking systems

<details>
<summary>Answer</summary>

**Correct: C**

Employment decisions are a regulated-decision category; using AI output as the sole determinant without human review violates responsible-use policy regardless of data handling, since such decisions carry legal and fairness implications.

**Why the others are wrong:**
- Claude can process bulk text; this is not a technical limitation question.
- PII handling is a separate concern from the appropriateness of automating the decision itself — even with properly redacted data, the automation issue remains.
- Output formatting is irrelevant to whether the use case is appropriate.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q4.** Why do many organizational AI policies impose restrictions stricter than Claude's baseline platform safeguards?

A) Anthropic requires every customer to write a custom policy before deployment
B) Organizations have additional legal, regulatory, and business-context obligations (e.g., industry compliance, contractual data handling terms) that a general-purpose platform cannot account for
C) Platform safeguards are being phased out in favor of organizational enforcement
D) Stricter policies are only needed for free-tier accounts, not enterprise agreements

<details>
<summary>Answer</summary>

**Correct: B**

Platform-level safeguards are designed for broad, general use; individual organizations operate under specific regulatory regimes (HIPAA, GDPR, financial regulations) and contractual obligations that require tighter, context-specific controls.

**Why the others are wrong:**
- There is no requirement from Anthropic mandating custom policy documents for deployment.
- Baseline safeguards remain in place regardless of organizational policy layering.
- Policy strictness is driven by organizational risk and regulatory context, not account tier.

</details>

---

**Q5.** An employee has a draft of unreleased quarterly financial projections. The company has not yet made this information public and only finance leadership has access. How should this data be classified before considering any AI tool use?

A) Public
B) Internal
C) Restricted/PII
D) Confidential

<details>
<summary>Answer</summary>

**Correct: D**

Unreleased financial projections with limited access and material business impact if disclosed fit the confidential classification — sensitive but not personal data (which would be restricted/PII).

**Why the others are wrong:**
- Public data is intended for open release; this data is explicitly not yet released.
- Internal data is broadly available to employees; this is restricted to finance leadership only, a tighter access tier.
- Restricted/PII specifically refers to personal identifiable information, not business financial data.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q6.** Before pasting a customer support ticket into Claude to draft a response, which anonymization step is MOST appropriate?

A) Leave all details intact since the ticket is only visible to the support agent
B) Delete the entire ticket text and ask Claude to guess the likely complaint
C) Replace the customer's name, email, and account number with generic placeholders (e.g., 'Customer A', 'email@example.com') while keeping the issue description intact
D) Translate the ticket into a different language to obscure identifying details

<details>
<summary>Answer</summary>

**Correct: C**

Redacting direct identifiers while preserving the operationally relevant content (the issue description) is the standard anonymization approach — it minimizes data exposure without destroying the task's usefulness.

**Why the others are wrong:**
- Visibility to one agent does not eliminate the data-handling risk of exposing PII to a third-party AI system.
- Removing all content defeats the purpose of using the tool and produces unusable output.
- Translation does not anonymize identifiers — names, emails, and account numbers remain in the translated text.

</details>

---

**Q7.** An employee is unsure whether using Claude to draft responses to regulatory inquiries falls within acceptable use under company policy. What is the correct next step?

A) Proceed since the policy does not explicitly forbid it
B) Avoid using Claude for anything related to the task going forward without asking anyone
C) Ask Claude itself whether the use case is compliant with company policy
D) Escalate the use case to the designated AI governance contact or committee for a policy determination before proceeding

<details>
<summary>Answer</summary>

**Correct: D**

Gray-area use cases — especially those touching regulatory matters — require escalation to the organization's designated AI governance contact or committee rather than individual judgment calls.

**Why the others are wrong:**
- Absence of an explicit prohibition does not equal approval; gray areas by definition require clarification.
- Avoiding the tool entirely without reporting the ambiguity bypasses the proper governance process and doesn't resolve the policy question for future use.
- Claude does not have authority over or visibility into the organization's internal policy and cannot make a binding compliance determination.

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q8.** Which pair of use cases correctly distinguishes appropriate from inappropriate use of Claude?

A) Appropriate: generating a final medical diagnosis for a patient; Inappropriate: drafting internal marketing copy for review
B) Both are appropriate as long as Claude's output is reviewed by any employee
C) Appropriate: drafting internal marketing copy for review; Inappropriate: generating a final medical diagnosis delivered to a patient without clinician review
D) Both are inappropriate because Claude cannot be used for any content involving health or marketing

<details>
<summary>Answer</summary>

**Correct: C**

Drafting content for human review is a low-risk, appropriate assistive use. Delivering an unreviewed medical diagnosis directly to a patient is a regulated, high-stakes decision requiring licensed professional oversight, making it inappropriate.

**Why the others are wrong:**
- Reversing the classification ignores the risk level difference between assistive drafting and autonomous high-stakes medical decisions.
- Review by 'any employee' is insufficient for regulated decisions like medical diagnosis, which require qualified clinical oversight, not general review.
- Marketing copy drafting for review is a standard appropriate use case and is not categorically prohibited.

</details>

---

