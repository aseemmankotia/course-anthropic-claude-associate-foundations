## Chapter 3 Cheat Sheet: Workflow Integration and Solution Design (16%)

### Step Classification Framework
| Classification | Definition | Example |
|---|---|---|
| AI-suitable | Claude can fully own the step, low risk if imperfect | Summarizing internal meeting notes for personal reference |
| Human-required | No AI involvement, accountability or judgment-critical | Final legal sign-off, irreversible financial transactions |
| Hybrid | Claude drafts/assists, human reviews and approves | Drafting support replies, drafting contract clauses |

**Exam rule of thumb:** when in doubt between AI-suitable and Hybrid, choose Hybrid if the output is customer-facing, irreversible, or compliance-sensitive.

### Research Modes
| Mode | Use case | Validation needed? |
|---|---|---|
| Exploratory | Early-stage brainstorming, surfacing options/angles | Yes — human validates before acting |
| Final-answer | Presenting a claim as settled fact | Always requires independent verification before this label is used |

**Exam trap:** requests like "give a definitive answer for the board" skip verification — flag this as a risk, not a capability limit.

### Process Optimization Checklist
- Identify repetitive, low-judgment steps first (drafting, summarizing, formatting).
- Keep irreversible actions (merge, publish, send, approve) with a human.
- Pilot on one step before scaling across the workflow.

### Framing AI Value — Do / Don't
| Do | Don't |
|---|---|
| "Claude accelerates first drafts; humans validate accuracy." | "Claude will replace the team." |
| State specific limits alongside benefits | "Claude never makes mistakes." |
| Tie value to a measurable step (e.g., drafting time) | Vague claims like "AI will transform everything" |

### Measuring Time Saved vs. Quality Trade-offs
- Track **two metrics together**: time saved on the automated portion AND any change in downstream review/correction time.
- A net positive requires total workflow time to improve **and** quality to hold steady or improve — not just faster first drafts.
- Common exam trap: assuming time saved alone proves successful integration; the exam expects you to weigh the trade-off, not just celebrate speed.

### Quick Memory Trick
**"D-V-A"** for any Hybrid step: Claude **D**rafts → Human **V**alidates → Human **A**pproves/acts.
