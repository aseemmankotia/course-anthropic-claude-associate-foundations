## Output Evaluation & Validation — Cheat Sheet

### Hallucination vs Outdated
| Type | Definition | Fix |
|---|---|---|
| Hallucination | Fabricated / never-true content | Remove, flag, re-verify from scratch |
| Outdated | Was once true, has since changed | Refresh with current source data |

### Risk Tiers → Review Requirement
| Tier | Example | Human Review |
|---|---|---|
| Low-stakes | Internal brainstorm, personal notes | Optional / spot-check |
| Medium-stakes | Internal report shared broadly | Recommended |
| High-stakes | Client-facing financial/legal/medical content | **Mandatory, full review** |

**Rule:** Review requirement scales with audience exposure × consequence of error — not output length or confidence of tone.

### Repeatable Fact-Check Pass (4 independent checks)
1. **Claims** — is the assertion itself true?
2. **Numbers** — does every figure match the source?
3. **Names** — are people/orgs/products named correctly?
4. **Dates** — are timeframes accurate and current?

Run each pass separately — catching one error type does not guarantee catching the others.

### Self-Verification Limits
- Claude's self-check = internal consistency check only.
- It is **never sufficient evidence** for high-stakes claims (citations, figures, legal/medical facts).
- Always escalate to an external primary source for high-stakes content.

### Bias Spotting Checklist
| Signal | Look For |
|---|---|
| Tone | Loaded/charged language favoring one side |
| Framing | What's emphasized first/last, what gets more detail |
| Omission | Missing perspectives, counterpoints, or context |

Omission bias is the hardest to catch — the page looks factually clean.

### Completeness Check
- Compare the scope of the question/source against the scope of the answer.
- Ask: "What did I actually ask vs what was actually answered?"
- Silent drops (e.g., 3 of 5 items listed) are a completeness failure, not a hallucination.

### Output Format Selection
| Format | Best For |
|---|---|
| Table | Comparing multiple items/metrics |
| Bullets | Scannable discrete points |
| Prose | Narrative reasoning, nuance, justification |

Choose based on audience consumption speed, not content type alone.

### Exam Traps
- Treating a passed self-verification as proof of accuracy (high-stakes trap).
- Confusing omission/framing bias with hallucination.
- Assuming confident tone correlates with correctness.
- Skipping the dates/names pass because the numbers checked out.
