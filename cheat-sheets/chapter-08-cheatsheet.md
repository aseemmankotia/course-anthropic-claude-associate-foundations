# Chapter 8 Cheat Sheet: Troubleshooting & Optimization

## Diagnostic Framework
| Step | Question | Action |
|---|---|---|
| 1 | What did I ask for vs. what did I want? | Compare literal prompt to intended outcome |
| 2 | Is context missing? | Add background, audience, data, constraints |
| 3 | Is the instruction ambiguous? | Specify scope, length, tone explicitly |
| 4 | Did I specify format? | State structure (list, table, JSON, prose) |

## Three Root Causes of Weak Output
- Missing context
- Ambiguous instructions
- Wrong or unspecified format request

## Clarifying Questions = Free Diagnostics
When Claude asks a clarifying question instead of answering, it is telling you exactly where your prompt was ambiguous. Incorporate the missing detail — don't resend the prompt unchanged.

## Fix Scope: One-Off vs. Systemic
| Symptom | Fix Location |
|---|---|
| Happens once | Edit the single prompt |
| Recurs across 3+ sessions | Edit custom instructions |
| Needs shared reference material every time | Add to Project knowledge base |

## Workflow Optimization Checklist (Post-Deployment)
- Remove reformatting steps by tightening the original format request
- Merge multi-prompt chains into single, well-specified prompts where possible
- Re-test after each trim to confirm output quality is unchanged
- Review stable workflows periodically — "it works" is not "it's optimized"

## Model/Surface vs. Prompt — Decision Table
| Symptom | Likely Cause | Fix |
|---|---|---|
| Vague, generic text | Missing context / ambiguous prompt | Rewrite the prompt |
| Repeated formatting drift | No persistent instruction | Add to custom instructions |
| Needs file/terminal access | Wrong surface | Use Claude Code / API with tools |
| Large document mishandled | Context limit exceeded | Chunk input; confirm against 200K token window |
| Same complaint across many sessions | Systemic, not one-off | Fix knowledge source or custom instructions |

## Key Numbers
- Standard context window: 200K tokens
- Few-shot fix for format drift: 2–3 examples typically sufficient

## Exact Fix Phrases
- Kill preamble: "Respond with only the requested content — no preamble."
- Kill markdown wrapping: "Output only raw [format], no code fences or extra commentary."
- Force structure: "Use exactly this structure: [heading] / [bullet list] / [table]."

## Exam Traps
- Assuming weak output means "switch to a bigger/different model" before checking for missing context or ambiguous instructions
- Re-editing a prompt every time instead of fixing custom instructions/knowledge sources for a recurring problem
- Adding more steps to a workflow instead of trimming redundant ones during optimization
- Blaming the prompt when the real issue is a surface lacking a needed capability (e.g., file/terminal access)
