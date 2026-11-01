## Chapter 4 Cheat Sheet: Governance, Risk, and Responsible Use (15%)

### Inappropriate Use Categories
| Category | Definition | Example |
|---|---|---|
| Regulated decisions | AI output as sole basis for high-stakes decision, no human review | Auto-rejecting job candidates |
| Deceptive content | AI output presented as authentic/human without disclosure | Fake customer testimonials |
| Unauthorized data sharing | Sensitive/PII data pasted into prompts without approval | Employee SSNs in a prompt |

**Rule of thumb:** If removing human oversight changes legal outcomes → regulated decision. If the audience is misled about authorship → deceptive content. If data leaves its approved boundary → unauthorized sharing.

### Data Sensitivity Classification
| Tier | Description | Example | AI Handling Rule |
|---|---|---|---|
| Public | Cleared for external release | Press releases | No restriction |
| Internal | Broad employee access, low external risk | Internal memos | Generally OK, org policy may still restrict |
| Confidential | Role-restricted, material harm if leaked | Unreleased financials | Requires approval; avoid in general prompts |
| Restricted/PII | Personal identifiers, legal protection | SSNs, health records | Redact/anonymize BEFORE any prompt use |

### Redaction Checklist (before pasting data)
1. Remove direct identifiers (name, SSN, email, account #)
2. Mask/generalize indirect identifiers (exact DOB → age range)
3. Keep only fields needed for the task
4. Confirm data classification allows AI tool use at all

### Responsible-AI Ethics (3 pillars)
- **Transparency** — disclose AI involvement in content
- **Fairness** — avoid biased/discriminatory outputs
- **Avoid deception** — never present AI output as human-authored without disclosure

### Policy Hierarchy Rule
Org policy is often STRICTER than platform baseline safeguards due to industry regulation (HIPAA, GDPR, finance) and contracts. **Always follow the stricter rule.**

### Gray-Area Escalation Path
1. Do NOT proceed based on 'not explicitly forbidden'
2. Do NOT ask Claude to self-certify compliance
3. Escalate to designated AI governance contact/committee
4. Wait for determination before using the use case in production

### Exam Traps
- 'Not explicitly prohibited' ≠ approved — always a wrong answer for gray areas
- Data format (PDF vs. text) does NOT change sensitivity classification
- Human review requirement doesn't disappear just because data was redacted (regulated-decision risk is separate from data-privacy risk)
- Switching to a personal account to bypass policy is always a violation, never a valid workaround
