## Chapter 7: Configuration and Knowledge Management — Practice Questions

**Q1.** A legal team creates a Claude Project to draft NDAs. They upload 40 old contract templates as knowledge and write custom instructions saying 'Always use formal legal tone and cite relevant clauses.' After a month, users complain that responses are inconsistent and sometimes ignore the tone instruction. What is the MOST likely cause?

A) The Project knowledge base has become too large and unfocused, diluting retrieval relevance
B) Custom instructions only apply to the first message in a conversation
C) Claude cannot read more than one uploaded document at a time
D) Custom instructions must be re-entered every session

<details>
<summary>Answer</summary>

**Correct: A**

A broad, unscoped knowledge base with many loosely related documents reduces retrieval precision — the model has to work across more conflicting context, which degrades consistency. Narrowing scope (fewer, more relevant documents) improves relevance.

**Why the others are wrong:**
- Custom instructions persist for the life of the Project, not just the first message
- Claude can use multiple uploaded documents in a Project's knowledge base simultaneously
- Custom instructions are stored at the Project level and do not need re-entry each session

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q2.** A company wants a Project where Claude can read and summarize new emails as they arrive, without the user manually uploading files. Which configuration should they use?

A) Connect the Gmail integration/connector to the Project
B) Upload exported .eml files to the Project knowledge base weekly
C) Add a custom instruction telling Claude to 'check email'
D) Create a new Project each time a new email arrives

<details>
<summary>Answer</summary>

**Correct: A**

Connectors (integrations) like Gmail pull live data from the connected account at query time, so Claude can access current emails without manual re-upload.

**Why the others are wrong:**
- Manually exporting and uploading files is static and does not reflect new incoming emails
- A custom instruction has no effect without an actual connector granting access — Claude cannot 'check email' on its own without the integration
- Creating a new Project per email is impractical and does not solve the live-access requirement

</details>

---

**Q3.** A marketing Project has a knowledge base containing the company style guide from 2023. The style guide was revised in 2026 with new brand voice rules, but the Project still produces outputs matching the old guide. What should the Project owner do?

A) Add a custom instruction telling Claude to ignore the old style guide
B) Delete the Project and start a new conversation
C) Replace the outdated style guide document in the knowledge base with the current version
D) Nothing — Claude automatically updates knowledge from the internet

<details>
<summary>Answer</summary>

**Correct: C**

Uploaded knowledge sources are static snapshots; they do not auto-update when the source document changes elsewhere. The owner must manually review and replace outdated files to keep the Project accurate.

**Why the others are wrong:**
- Telling Claude to 'ignore' a document still leaves outdated content in the context and is unreliable compared to simply replacing it
- Deleting the whole Project loses custom instructions and other valid knowledge unnecessarily
- Uploaded knowledge files are not live-synced to the internet or re-fetched automatically

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q4.** Which of the following is a valid custom instruction use case for a Project, as opposed to a knowledge source?

A) A requirement that Claude always respond in bullet points and avoid jargon
B) A 50-page product manual
C) A spreadsheet of customer order history
D) A PDF of legal terms and conditions

<details>
<summary>Answer</summary>

**Correct: A**

Custom instructions define recurring behavior, tone, role, and constraints (such as formatting rules), while knowledge sources are reference documents/data the model reads from.

**Why the others are wrong:**
- A product manual is reference material, best stored as a knowledge source, not an instruction
- A spreadsheet of order history is data/content, not a behavioral instruction
- A terms-and-conditions PDF is reference content, appropriate for the knowledge base

</details>

---

**Q5.** A workspace admin shares a Project with the whole team. One team member reports that Claude cannot access the Google Drive files connected to the Project, even though the admin set up the connector. What is the MOST likely reason?

A) Google Drive connectors only work for the Project creator, never other members
B) The Project needs to be recreated for each team member
C) Google Drive connectors are deprecated and no longer supported
D) The team member has not individually authorized their own connection/permissions for the connector

<details>
<summary>Answer</summary>

**Correct: D**

Connected data access is typically tied to each individual user's own OAuth authorization and permissions — sharing a Project does not automatically grant another user's account access to the connector; each member generally must connect their own account.

**Why the others are wrong:**
- Shared Projects are meant to be usable by team members, not restricted solely to the creator, once each member authorizes access
- Recreating the Project is unnecessary — the fix is authorizing the connector per user
- Google Drive is an actively supported connector, not deprecated

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q6.** A Project was originally scoped broadly as a 'general company assistant' with instructions covering HR policy, sales scripts, and engineering onboarding. Users report irrelevant or generic answers. What is the recommended fix based on scoping best practices?

A) Split the Project into narrower, department-specific Projects
B) Add more custom instructions to cover even more departments
C) Increase the number of uploaded documents in the single Project
D) Remove all custom instructions and rely only on default behavior

<details>
<summary>Answer</summary>

**Correct: A**

Narrowly scoped Projects with tightly relevant instructions and knowledge produce more relevant, consistent outputs than one broad, catch-all Project covering unrelated domains.

**Why the others are wrong:**
- Adding more instructions to an already overloaded, broad Project worsens relevance rather than fixing it
- Adding more documents increases scope further instead of narrowing it, compounding the problem
- Removing instructions entirely would also remove the useful tone/role constraints that help relevance

</details>

---

**Q7.** A Project's custom instructions still say 'Always reference the Q1 2024 sales targets' even though the company is now tracking Q1 2026 targets. What should be done to keep the Project configuration current?

A) Leave it unchanged since custom instructions cannot be edited after creation
B) Start a new conversation thread, which automatically clears old instructions
C) Add a knowledge source correcting the date, without touching the instructions
D) Review and edit the custom instructions to remove or update the outdated reference

<details>
<summary>Answer</summary>

**Correct: D**

Custom instructions should be periodically reviewed and updated as business needs change; outdated instructions that reference stale data should be edited or removed to prevent incorrect or confusing responses.

**Why the others are wrong:**
- Custom instructions are editable at any time — this is a core part of maintaining a Project
- A new conversation thread within the same Project still inherits the Project's existing custom instructions
- Adding a correcting knowledge source without updating the instruction leaves a direct contradiction in the Project configuration

> ⚠️ Frequently missed on the exam — read the options carefully.

</details>

---

**Q8.** What is the primary difference between a Project's custom instructions and its connected knowledge sources?

A) Custom instructions define behavior/tone/constraints; knowledge sources provide reference content and data
B) Custom instructions are only visible to admins; knowledge sources are visible to all users
C) Custom instructions expire after 30 days; knowledge sources do not
D) Knowledge sources can only be text; custom instructions can include files

<details>
<summary>Answer</summary>

**Correct: A**

Custom instructions configure how Claude behaves (tone, role, recurring constraints), while knowledge sources supply the material Claude references when answering — this is the fundamental conceptual distinction tested on the exam.

**Why the others are wrong:**
- Visibility is governed by Project sharing/access settings, not an inherent split between instructions and knowledge
- Custom instructions do not have a fixed expiration period
- Knowledge sources support various document types, and custom instructions are text-based configuration, not file attachments

</details>

---

