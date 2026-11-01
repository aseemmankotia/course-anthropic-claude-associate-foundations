## Chapter 7 Cheat Sheet — Configuration & Knowledge Management (12% of exam)

### Custom Instructions vs. Knowledge Sources vs. Connectors
| Element | What it does | Updates? | Example |
|---|---|---|---|
| Custom Instructions | Sets tone, role, recurring constraints/behavior | Manually edited, persists until changed | "Always respond formally, cite sources" |
| Knowledge Sources (uploaded) | Static reference docs/data Claude reads from | Static snapshot — does NOT auto-update | Style guide PDF, product manual |
| Connectors/Integrations | Live external data access (Google Drive, Gmail, etc.) | Dynamic — pulled at query time | Gmail inbox, Drive folder |

**Exam rule of thumb:** If the use case needs *current/live* data → connector. If it needs *stable reference material* → knowledge upload. If it needs *behavioral consistency* → custom instructions.

### Scoping Guidance
- **Narrow scope** (one domain, task-specific knowledge + instructions) → higher relevance, more consistent output.
- **Broad scope** (multiple unrelated domains crammed into one Project) → generic/inconsistent answers, diluted retrieval.
- **Fix for "too broad"**: split into multiple narrowly scoped Projects rather than adding more instructions/docs to one.

### Maintenance Checklist
1. **Review knowledge sources periodically** — if the source-of-truth document changed externally, the uploaded copy in the Project is stale until manually replaced.
2. **Audit custom instructions** when business rules, dates, or policies change — remove/edit anything outdated or contradictory.
3. **Re-test Project outputs** after any instruction or knowledge change to confirm desired behavior.

### Connectors: Access & Sharing
- Connecting Google Drive/Gmail grants Claude access based on the **connecting user's own permissions/OAuth grant**.
- Sharing a Project with teammates does **not** automatically share connector access — each collaborator typically must authorize their **own** connection.
- Common exam trap: assuming a shared Project universally shares connected data access for all members — it doesn't.

### Common Exam Traps
- Confusing "knowledge source" (static content) with "connector" (live data) — know which solves which scenario.
- Assuming uploaded knowledge auto-refreshes when the original document changes — it does not; manual replacement required.
- Overloading one Project with unrelated instructions/knowledge instead of splitting into narrower Projects — causes relevance drift.
- Forgetting that each team member usually needs their own connector authorization even in a shared Project.
- Leaving outdated custom instructions unedited after requirements change, causing contradictory or wrong-toned output.

### Quick Decision Tree
- Need live/current external data? → **Connector** (Drive, Gmail)
- Need stable reference material (guides, manuals, policies)? → **Knowledge Source**
- Need consistent tone/role/formatting across all chats in the Project? → **Custom Instructions**
- Project outputs feel generic/inconsistent? → **Check scope** — narrow it down.
