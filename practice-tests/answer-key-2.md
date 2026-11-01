# Answer Key — Practice Test 2

**Q1. Correct: B**

Hallucinated case citations are a well-documented LLM failure mode. Perfectly formatted citations can still refer to nonexistent or misstated cases, so the only reliable check is independent verification against an authoritative legal database.

---

**Q2. Correct: C**

A specific, confidently-stated statistic with a false attribution to a nonexistent study is a classic hallucination. It should be removed or flagged and replaced with a verified source, not reworded or trusted.

---

**Q3. Correct: C**

A fixed JSON schema is machine-parseable and allows automated schema validation (correct field names, types, presence) before downstream processing, catching malformed output before it breaks the pipeline.

---

**Q4. Correct: B**

Since LLMs lack reliably calibrated self-confidence, the recommended practice is defining risk-based rules tied to domain impact (e.g., medical, legal, financial) and routing those categories to mandatory human review regardless of surface tone.

---

**Q5. Correct: D**

This reflects proper output bias mitigation: investigate for a systematic pattern across a larger sample, adjust prompting toward objective achievement-based language, and keep human review in the loop for a sensitive, high-impact use case like hiring.

---

**Q6. Correct: B**

This correctly separates the two failure modes: hallucination concerns factual fabrication/incorrectness, while bias concerns unfair or unbalanced framing, selection, or representation even when facts are technically accurate.

---

**Q7. Correct: B**

Claude's fluency and confident tone are not reliable signals of factual accuracy, especially for precise details like page numbers, which are a common hallucination point. The only dependable validation method for high-stakes, fact-based claims is manual verification against the authoritative source.

---

**Q8. Correct: A**

School prestige, zip code, and similar details can act as proxies for protected characteristics even without explicit demographic data. Bias in this kind of output requires structured human review of the decision criteria and rationale, not blind trust or a vague reprompt, before it influences real hiring outcomes.

---

**Q9. Correct: B**

Clinical dosage recommendations carry direct risk to patient safety if incorrect, and Claude is not a licensed medical authority with guaranteed accuracy on individualized medical calculations. Any output with high real-world stakes and potential for harm — especially in regulated domains like healthcare — mandates review by a qualified human expert before being acted on.

---

**Q10. Correct: A**

Claude is well-suited for first-pass clause flagging and summarization (research/process optimization), but autonomous final approval on consequential legal decisions removes human judgment from a high-risk step, which is exactly the kind of boundary a CCAO-F practitioner must identify and communicate to a team.

---

**Q11. Correct: D**

Given both documents are relatively short and the task is extraction plus comparison plus drafting, a single well-structured prompt with both documents in context, followed by human sign-off, is an efficient and appropriately-scoped design that keeps a human in the loop for the final decision.

---

**Q12. Correct: C**

This design uses Claude where it adds clear value — categorization and drafting, which are high-volume and low-risk — while keeping humans responsible for consequential or irreversible actions like refunds and account changes, which matches how CCAO-F frames appropriate human-in-the-loop boundaries.

---

**Q13. Correct: C**

A human checkpoint before downstream action is the standard, reliable mitigation for output-quality risk in an automated pipeline; it directly addresses the consequence of an error (bad data entering the ticketing system) rather than trying to eliminate the underlying model limitation.

---

**Q14. Correct: D**

Chaining the work into a summarize-then-synthesize pattern with intermediate review improves traceability and accuracy, and is a more robust process-optimization design than relying on one large undifferentiated pass, especially when it matters that each source's contribution can be checked.

---

**Q15. Correct: A**

A core limitation to communicate is that fluent, confident-sounding output is not the same as verified accuracy — this is a well-known failure mode where users over-trust well-written responses, and it directly affects how research outputs should be reviewed before being relied upon.

---

**Q16. Correct: A**

Claude's knowledge and reasoning operate on the context it is given; it has no built-in persistent connection to live external databases or systems of record. Confirming a 'current' signature status requires real-time ground truth, which Claude cannot provide unless explicitly integrated via tool use/function calling or given a fresh data feed in the prompt. This is a classic case where the workflow step depends on live system state rather than language understanding, making it unsuitable for Claude alone.

---

**Q17. Correct: A**

Enterprise/Team agreements include contractual data protections (e.g., no training on prompts, DPA, retention controls) appropriate for regulated PHI, and de-identifying sensitive data further reduces risk regardless of tool.

---

**Q18. Correct: A**

Anthropic's Usage Policy requires human oversight for high-stakes outputs such as medical content — Claude can assist, but a qualified professional must validate outputs before they reach a patient.

---

**Q19. Correct: A**

The RSP defines capability thresholds (increasing AI Safety Levels) with corresponding security and deployment safeguards designed to manage catastrophic risk as model capabilities scale.

---

**Q20. Correct: D**

Anthropic's commercial terms state that API inputs and outputs are not used for model training by default, and are retained only for a limited window (e.g., trust & safety review) unless the customer opts in or law requires otherwise.

---

**Q21. Correct: C**

Fully automating consequential, adverse employment decisions without human review removes accountability and can embed or amplify bias undetected — a core governance concern for high-stakes, consequential AI decisions.

---

**Q22. Correct: B**

Transparency and disclosure of AI-generated content is a recognized responsible-AI governance practice, and increasingly a legal/policy requirement, to maintain reader trust and informed consent.

---

**Q23. Correct: B**

A contracted API deployment with a signed data processing agreement and zero data retention satisfies the policy's explicit requirement for contractual data commitments, which consumer products lack regardless of how the chat is handled afterward.

---

**Q24. Correct: D**

Requiring Claude to ground each risk in a direct quote, structured with XML tags, forces verifiable grounding to source text and lets the reviewer check each claim against the exact clause, directly reducing unverifiable summarization.

---

**Q25. Correct: A**

Multishot prompting with concrete labeled examples anchors Claude to the exact desired input/output format and category boundaries, which is the most reliable way to achieve consistent, parseable classification at scale.

---

**Q26. Correct: A**

Prefilling the start of the Assistant turn (e.g., with '{') causes Claude to continue generation from that point, skipping any conversational preamble and reliably producing output that starts exactly where the prefill left off.

---

**Q27. Correct: B**

Decomposing a large, multi-stage task into sequential steps with checkpoints (outline approval, section-by-section drafting, dedicated editing) lets the user catch errors early, keeps each prompt focused, and produces materially higher quality than a single monolithic request.

---

**Q28. Correct: B**

The system prompt is designed to establish persistent context, role, and behavior guidelines that persist for the duration of the interaction, whereas user turn content is the specific, per-turn request Claude is asked to act on.

---

**Q29. Correct: D**

Effective iteration requires specific, actionable feedback — naming the exact problem (tone), showing a concrete example of the desired result, and pointing to the affected content — which gives Claude the information needed to make a targeted correction while preserving the already-correct factual content.

---

**Q30. Correct: C**

Projects let users attach persistent documents to a shared knowledge base that is automatically available across all conversations within that Project, and the source documents can be updated centrally without re-uploading them each time.

---

**Q31. Correct: C**

Artifacts render substantial, self-contained content (like React components, documents, or diagrams) in a dedicated side panel that updates as the content is iterated on, separate from the back-and-forth chat text.

---

**Q32. Correct: C**

Haiku is Anthropic's fastest and most cost-efficient model, purpose-built for high-volume, low-complexity tasks like simple classification where latency and per-call cost at massive scale matter most.

---

**Q33. Correct: D**

When content exceeds a model's context window regardless of which model is chosen, the standard approach is chunking: process sections individually (summarize/extract), then feed those condensed intermediate results back to Claude for final synthesis — preserving coverage of the whole archive.

---

**Q34. Correct: B**

The request depends on up-to-date, time-sensitive information from multiple external sources published very recently, which is exactly what research mode is designed to handle via live multi-step web search and synthesis — standard chat alone cannot reliably know events from the last two weeks.

---

**Q35. Correct: C**

Documents added to a Project's knowledge base are static snapshots at upload time. Unlike connectors, they do not refresh automatically — the file must be manually re-uploaded or replaced to reflect source changes.

---

**Q36. Correct: A**

The Gmail connector gives Claude on-demand access to live inbox content, which is necessary when source data changes frequently throughout the day.

---

**Q37. Correct: C**

Custom instructions are explicit behavioral configuration that governs how Claude responds across the Project. Uploaded knowledge documents are reference material for facts and context, not instructions on tone or style, so instructions take precedence.

---

**Q38. Correct: D**

Project custom instructions are a persistent configuration applied to every new conversation started inside that Project, providing consistent behavior across all chats, whereas settings scoped to one conversation do not carry over to others.

---

**Q39. Correct: D**

Organization-level admin controls in Claude Enterprise take precedence over individual user connector authorizations. Disabling a connector at the org level revokes access across all Projects and users, not just new ones.

---

**Q40. Correct: D**

Anthropic's documented long-context guidance recommends placing long documents or data first, with instructions and the question immediately after. This reduces the 'lost in the middle' effect and puts the question closer to generation, improving recall of details buried in the middle of long inputs.

---

**Q41. Correct: A**

Prefilling the assistant turn with the opening of the desired output (e.g., "{") is a documented Anthropic technique that forces Claude to continue directly from that point, bypassing conversational preamble and reliably enforcing output format.

---

**Q42. Correct: D**

Setting temperature near 0 minimizes randomness in token sampling, producing the most consistent and reproducible outputs across repeated calls with identical input — exactly what a regression test suite needs.

---

**Q43. Correct: C**

The max_tokens parameter caps the length of the generated response. If output is being truncated mid-sentence while input context is well within limits, the response is hitting the max_tokens ceiling, and increasing it is the direct fix.

---

**Q44. Correct: B**

A systematic evaluation dataset that covers the diversity of real-world inputs exposes edge cases and failure patterns before launch, which ad-hoc manual testing on a handful of examples cannot reveal.

---

