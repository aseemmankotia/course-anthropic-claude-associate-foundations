# Answer Key — Practice Test 1

**Q1. Correct: D**

Claude can fabricate plausible-sounding but nonexistent case citations, docket numbers, and statutes (a known hallucination pattern). Specific, checkable factual claims like legal citations must be independently verified against an authoritative source before use, especially in high-stakes domains like law.

---

**Q2. Correct: A**

When output must be machine-parsed reliably, requesting a strict JSON schema with an explicit instruction to suppress extra prose minimizes parsing errors and ambiguity, making it the most robust choice for programmatic consumption.

---

**Q3. Correct: C**

High-stakes domains like medical diagnosis always require human-in-the-loop review by a qualified professional, independent of output quality, confidence, or caveats, because the cost of an undetected error is severe and Claude is not a licensed clinical decision-maker.

---

**Q4. Correct: B**

Hallucinations most commonly manifest as specific, checkable details — dates, numbers, names, citations — that are fabricated but presented in the same style as accurate ones. The presence of such unverifiable specifics is the actionable signal that should trigger fact-checking.

---

**Q5. Correct: C**

Counterfactual testing — holding content constant while varying only a demographic attribute — isolates whether that attribute changes the output, which is the standard, rigorous method for surfacing systematic bias.

---

**Q6. Correct: D**

Completeness checking requires explicitly comparing the output against every component of the original request; silently dropped sub-questions are a known failure mode, and the reviewer must flag and resolve the gap rather than assume the task is finished.

---

**Q7. Correct: C**

High-stakes, externally-facing outputs that contain specific factual claims (dates, amounts, obligations) require human verification against the authoritative source before use — direct quoting does not guarantee the model didn't drop, alter, or misattribute a detail during summarization.

---

**Q8. Correct: A**

Schema-conformant JSON gives a machine-parseable, consistently structured format that a downstream script can validate programmatically (required keys, types) before insertion, catching malformed or missing fields automatically.

---

**Q9. Correct: D**

Claude can generate plausible-looking but fabricated citations (including fake authors, years, page numbers, or statistics) with high confidence; the only reliable check is to independently locate the actual source and confirm the citation and figure genuinely exist and match.

---

**Q10. Correct: C**

Finalizing a client-facing investment recommendation carries fiduciary and regulatory accountability, requiring human sign-off even if Claude drafts a version first.

---

**Q11. Correct: D**

Projects persist uploaded files and context as Project knowledge, making it automatically available in every conversation within that Project without re-uploading.

---

**Q12. Correct: B**

Project-level custom instructions function as a persistent system-level directive applied automatically to every conversation started within that Project.

---

**Q13. Correct: C**

Policy-exception financial approvals carry accountability and risk that require human judgment and sign-off, making this the least appropriate task for full autonomy.

---

**Q14. Correct: C**

Without tools or search enabled, Claude relies on its training data, which has a knowledge cutoff, making it unreliable for real-time or very recent information.

---

**Q15. Correct: A**

This statement accurately balances Claude's strengths in accelerating knowledge work with the ongoing need for human verification on factual or high-stakes outputs.

---

**Q16. Correct: A**

Claude is well-suited to high-volume, well-defined tasks like clause extraction and summarization, which speeds up review while reducing manual effort. However, final legal risk sign-off carries accountability and liability implications that require human judgment, domain expertise, and the ability to be held responsible for the decision — a known limit of relying on Claude for high-stakes final decisions.

---

**Q17. Correct: B**

Sensitive personal data (PII, medical, compensation) should be minimized or anonymized before being shared with any AI tool, and organizations should rely on enterprise agreements with defined data handling and retention terms when processing such data.

---

**Q18. Correct: D**

For high-stakes, safety-critical, or regulated outputs, responsible use requires qualified human review before deployment, since AI-generated content can contain errors with serious real-world consequences.

---

**Q19. Correct: C**

Organizational AI policies exist to manage legal, contractual, and data-protection risk; employees should follow policy and escalate through proper channels (e.g., IT, legal, procurement) rather than finding workarounds.

---

**Q20. Correct: B**

When contractual guarantees on data handling, retention, and training exclusion are required, an enterprise or business agreement with clearly defined terms is the appropriate choice, rather than consumer-tier products.

---

**Q21. Correct: B**

Loan eligibility decisions are high-stakes and can significantly affect individuals' financial lives, so responsible deployment requires human oversight and an escalation path rather than fully automated, unreviewed decisions.

---

**Q22. Correct: A**

Diverse review perspectives help surface biases or harms that may not be apparent to a homogeneous reviewer group, improving fairness and reducing the risk of harmful outputs reaching end users.

---

**Q23. Correct: A**

Removing or masking personally identifiable and financial information before sending data to any AI system is a core data-sensitivity practice — the request can usually be rephrased generically (e.g., 'a customer,' '[ADDRESS]', '[CARD NUMBER]') without losing the context needed for Claude to draft a helpful reply.

---

**Q24. Correct: A**

Specifying an exact schema and systematic extraction categories reduces ambiguity and ensures complete, consistently formatted output suited to structured data extraction from a long document.

---

**Q25. Correct: C**

Sequential, verifiable steps (generate, then test, then fix) let you catch and correct issues iteratively, matching the task decomposition approach recommended for multi-step technical work.

---

**Q26. Correct: D**

Explicit step-by-step reasoning before stating the final answer lets the model externalize intermediate calculations, which is a core recommended technique for improving accuracy on multi-step reasoning tasks.

---

**Q27. Correct: B**

Combining explicit schema instructions with prefilling the assistant response (starting with "{") is a documented technique that reliably constrains output format and prevents preamble or trailing text.

---

**Q28. Correct: D**

Low temperature favors deterministic, precise outputs suited to factual extraction, while a higher temperature introduces useful variability for creative, divergent tasks like tagline brainstorming.

---

**Q29. Correct: A**

Task decomposition means splitting a complex objective into smaller, manageable, verifiable steps, which improves reliability and allows catching errors early in multi-step workflows.

---

**Q30. Correct: B**

Haiku is Anthropic's fastest and cheapest model, purpose-built for high-volume, low-latency tasks like simple classification, making it the most cost-effective choice at 50,000 requests/day.

---

**Q31. Correct: B**

Research mode is designed for multi-step, iterative web research, pulling from multiple sources and synthesizing a cited report — exactly the workflow described.

---

**Q32. Correct: D**

Artifacts creates a dedicated side panel for generated content like code or prototypes, allowing the user to view and iterate on the output separately from the conversation — the exact workflow described.

---

**Q33. Correct: D**

Projects allows teams to upload knowledge base files and custom instructions that persist and are automatically available across every conversation started within that project — exactly the shared-context need described.

---

**Q34. Correct: B**

Claude 3 family models (Haiku, Sonnet, Opus) ship with a standard 200,000-token context window, enabling processing of long documents or extended conversations.

---

**Q35. Correct: C**

Custom Instructions are applied automatically to every conversation inside a Project, making them the correct mechanism for enforcing consistent tone, format, and behavior across all chats without repeating instructions.

---

**Q36. Correct: A**

The Google Drive connector gives Claude access to the live, current version of documents, eliminating the need to manually re-upload files whenever content changes.

---

**Q37. Correct: A**

Project Knowledge has a finite capacity shown as a usage indicator in the interface; once full, existing files must be removed or replaced before new files can be added.

---

**Q38. Correct: C**

Custom Instructions define behavioral guidance — tone, persona, format, constraints — applied to every chat in the Project, while Project Knowledge is a repository of reference material (documents, files) Claude consults for factual content.

---

**Q39. Correct: C**

Maintaining a Project over time requires periodic review of connector access and stored knowledge so outdated or irrelevant content is removed, keeping responses accurate and relevant.

---

**Q40. Correct: B**

Few-shot examples, especially structured with XML tags, give Claude a concrete template for format and length, which is the standard fix for inconsistent output structure.

---

**Q41. Correct: A**

Explicitly grounding instructions that restrict Claude to the provided context, with an explicit fallback for missing information, is the recommended technique for reducing hallucination in RAG workflows.

---

**Q42. Correct: D**

The Console's Evaluate tool lets teams build a test suite of representative inputs, run prompt variants against them, and compare results systematically before deployment.

---

**Q43. Correct: B**

For simple, well-defined tasks like binary classification, switching to a smaller model like Haiku substantially reduces latency and cost while maintaining accuracy, since the task doesn't require the deeper reasoning capacity of larger models.

---

**Q44. Correct: D**

Isolating variables by changing one prompt element at a time and re-testing lets you attribute performance changes to a specific cause, which is the standard systematic debugging approach for prompts.

---

