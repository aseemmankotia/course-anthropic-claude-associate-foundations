## Chapter 7: Configuration and Knowledge Management — Flashcards

| # | Front (Question) | Back (Answer) |
|---|-----------------|---------------|
| 1 | What do Custom Instructions configure in a Claude Project? | Tone, role, and recurring constraints that apply across every conversation in that Project. Exam tip: instructions = behavior, not reference content. |
| 2 | What do Knowledge Sources provide in a Claude Project? | Reference documents, style guides, and data Claude reads from when answering within that Project. Static unless paired with a connector. |
| 3 | Uploaded knowledge files vs. connectors — which auto-updates? | Connectors (e.g., Gmail, Google Drive) pull live data at query time. Uploaded files are static snapshots and must be manually replaced when sources change. |
| 4 | A Project owner updates a source document externally. Does the Project's uploaded copy update automatically? | No. Uploaded knowledge is a static snapshot — the owner must manually re-upload/replace the file to reflect changes. |
| 5 | Narrow scoping vs. broad scoping a Project — which improves relevance? | Narrow scoping (one domain/task, tightly relevant knowledge and instructions) improves retrieval relevance and consistency over broad, catch-all Projects. |
| 6 | Symptom: inconsistent or generic answers from a Project with lots of unrelated documents and instructions. | Likely caused by overly broad scope. Fix: split into narrower, purpose-specific Projects. |
| 7 | Two examples of connectors/integrations commonly tested for Claude Projects. | Google Drive and Gmail (also commonly tested alongside Google Calendar and other workspace tools) — these provide live external data access, unlike static uploads. |
| 8 | Team member can't access Project's connected Google Drive data despite the Project being shared. Why? | Connector access is typically tied to each individual user's own authorization/permissions — sharing a Project doesn't automatically grant another user's account access to the connector. |
| 9 | When should custom instructions be reviewed/removed? | Whenever business needs change — outdated references (old dates, deprecated policies) should be edited or removed to avoid incorrect or contradictory responses. |
| 10 | Custom instruction references stale data (e.g., old fiscal year). Best fix? | Edit/update the custom instructions directly — they are editable at any time and should be kept current, not left unchanged or patched only via new knowledge. |
| 11 | Knowledge source: 50-page product manual. Custom instruction: 'respond in bullet points.' Which is which? | Manual = knowledge source (reference content). 'Respond in bullet points' = custom instruction (behavioral constraint). |
| 12 | Why can a Project with a connected data source raise access/sharing concerns? | Connected data often inherits the permissions of the connecting account; sharing the Project doesn't share the underlying data access automatically — each collaborator may need their own authorized connection. |
