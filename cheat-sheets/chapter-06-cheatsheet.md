## Chapter 6 Cheat Sheet: Product & Model Selection (12%)

### Product Selection
| Product | Use When | Key Trait |
|---|---|---|
| **Chat** | Quick, one-off task | No persistent context between sessions |
| **Projects** | Ongoing, context-rich work | Persistent knowledge base + custom instructions across sessions |
| **Research mode** | Multi-source exploratory questions | Synthesizes info across sources, provides citations |
| **Artifacts** | Need standalone, reusable output | Generates editable structured content (code/docs/reports) in separate pane |

**Exam Rule:** Match keywords —
- "one-time" / "quick" → Chat
- "repeated" / "ongoing" / "shared context" → Projects
- "gather from multiple sources" / "synthesize" → Research mode
- "standalone" / "reusable document" → Artifacts

### Model Selection
| Model | Speed | Cost | Best For |
|---|---|---|---|
| **Haiku** | Fastest | Lowest | Simple, high-volume tasks (classification, short replies) |
| **Sonnet** | Balanced | Mid | Default everyday knowledge work (drafting, coding, analysis) |
| **Opus** | Slowest | Highest | Complex reasoning, nuanced judgment, highest accuracy needs |

**Exam Rule:** If priority = cost/speed → Haiku. If priority = balance/default → Sonnet. If priority = max accuracy/complex reasoning → Opus.

### Context Window
- All three models (Haiku, Sonnet, Opus) share the **same context window (~200K tokens)** as of 2026.
- Model tier affects **capability/speed/cost**, NOT context window size.
- **Extremely long documents** exceeding the window must be **chunked**, or use a **Project's knowledge base** for retrieval rather than pasting the full text at once.

### Common Exam Traps
1. Using **Opus** for simple, high-volume tasks → wasteful, wrong answer.
2. Using **Haiku** for complex, nuanced reasoning → underpowered, wrong answer.
3. Assuming a higher-tier model has a **bigger context window** — it does not; window size is constant across tiers.
4. Choosing **Chat** for recurring work that needs persistent context — should be **Projects**.
5. Choosing **Research mode** when the task is generating a deliverable (should be **Artifacts**), or vice versa.

### Quick Decision Flow
1. Is this **one-off**? → Chat
2. Is this **recurring with shared context**? → Projects
3. Does it need **multi-source synthesis**? → Research mode
4. Does it need a **standalone deliverable**? → Artifacts
5. Then pick model based on **task complexity vs. cost/speed priority**: Haiku (simple/cheap) → Sonnet (default) → Opus (complex/high-accuracy).
