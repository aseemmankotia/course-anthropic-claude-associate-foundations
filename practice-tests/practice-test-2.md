# Practice Test 2: CCAO-F: Claude Certified Associate Foundations Exam Prep

- **Questions:** 44
- **Time limit:** 90 minutes
- **Passing score:** 70%%

> Answers are in `answer-key-2.md`. Track results in `score-tracker.md`.

---

**Q1.** A paralegal uses Claude to draft a legal memo and asks it to cite relevant case law. Claude returns a memo with five case citations, including full case names, years, and court names, all formatted correctly. Which validation step is MOST important before the memo is used?

A) Re-run the same prompt to see if Claude returns consistent citations
B) Independently verify each citation exists in a legal database like Westlaw or Lexis
C) Ask Claude to confirm that the citations are accurate
D) Check that citation formatting follows Bluebook style

---

**Q2.** During review, an analyst notices that Claude's output states 'According to a 2024 McKinsey study, 73% of enterprises adopted AI governance frameworks,' but no such study or statistic can be found despite the confident, specific tone. What is this error type, and what should the analyst do?

A) This is a bias error; the analyst should ask Claude to rephrase more neutrally
B) This is a formatting error; the analyst should ask Claude to add a citation
C) This is a hallucination; the analyst should remove or flag the unverifiable claim and request a real source
D) This is expected behavior since Claude cannot access real-time data, so the statistic should be trusted as a reasonable estimate

---

**Q3.** A team is building an automated pipeline where Claude extracts invoice fields (vendor, amount, due date) that are parsed by downstream Python code. Which instruction to Claude BEST ensures reliable automated validation of the output?

A) Instruct Claude to write a friendly paragraph summarizing the invoice details
B) Instruct Claude to output a markdown table since it's human-readable
C) Instruct Claude to output a JSON object with a fixed schema and specific field names, and validate the response against that schema before parsing
D) Instruct Claude to output plain text with labeled fields separated by commas

---

**Q4.** Since Claude does not expose a native numeric confidence score with its responses, which approach is the MOST reliable way to decide when an output requires mandatory human review in a production pipeline?

A) Ask Claude at the end of its response to rate its own confidence from 1-10 and use that score to trigger review
B) Define domain-specific risk rules (e.g., any output involving medical dosages, legal advice, or financial figures above a threshold) and route those categories to mandatory human review regardless of how the output reads
C) Trust outputs that are longer and more detailed, since detail indicates higher confidence
D) Only route outputs to human review when Claude explicitly says 'I'm not sure' or similar hedging language

---

**Q5.** A hiring team uses Claude to summarize candidate resumes for a shortlist. Reviewing the outputs, a diversity officer notices summaries describing candidates with traditionally masculine-associated names using words like 'driven' and 'assertive,' while candidates with traditionally feminine-associated names are described as 'organized' and 'supportive' for similar achievements. What is the BEST response?

A) Ignore the pattern since Claude is not capable of bias, only humans introducing bias into prompts
B) Ask Claude to confirm whether it was biased, and proceed based on its self-assessment
C) Discontinue using Claude for this entire use case permanently, since any detected bias means the tool is unusable for HR purposes
D) Treat this as a potential output bias issue: review a larger sample for systematic patterns, adjust prompts to request objective achievement-based language, and have a human review summaries before use in hiring decisions

---

**Q6.** Which statement BEST distinguishes a hallucination from a bias issue in Claude's output?

A) A hallucination is always more harmful than bias, so it should always be prioritized first in review
B) A hallucination is fabricated or factually incorrect content presented as true; bias is a systematic skew in how content is framed, selected, or represented that may be factually accurate but unfair or unbalanced
C) Hallucination only occurs in creative writing tasks, while bias only occurs in factual tasks
D) Bias and hallucination are two terms for the same underlying model failure and can be used interchangeably

---

**Q7.** A compliance analyst asks Claude to review a 50-page vendor contract and list every indemnification clause along with the exact page number where it appears. Claude returns a confident, well-formatted summary with specific page citations for each clause. What is the most reliable way to validate this output before the analyst relies on it in a filing?

A) Trust the citations as-is, since Claude's confident, fluent phrasing indicates the page numbers are well-calibrated to its actual certainty
B) Manually cross-reference every cited page number and clause against the actual source document, since Claude can hallucinate specific details like page numbers even when the surrounding text sounds authoritative
C) Ask Claude to self-rate its confidence in the citations on a 1-10 scale and accept the output if it rates 7 or higher
D) Re-run the identical prompt once more; if the second response lists the same page numbers, treat that consistency as proof of accuracy

---

**Q8.** An HR team uses Claude to rank job candidates from resumes for a technical role. A reviewer notices the top-ranked candidates disproportionately attended a small set of universities, even though prior experience and skills appear comparable across candidates. What is the correct next step?

A) Require human review of the ranking criteria, specifically checking whether proxy variables like university name or zip code are driving the outcome, before any hiring decision is finalized
B) Accept the ranking as unbiased because Claude was never given protected attributes like race or gender
C) Automatically discard the ranking and instruct Claude in a follow-up prompt to simply 'be fair this time'
D) Trust the ranking since it was generated purely from resume text, which is considered objective input

---

**Q9.** Which of the following Claude-generated outputs REQUIRES mandatory human expert review before anyone acts on it?

A) A marketing tagline Claude drafted for an internal brainstorming session, to be discussed and voted on by the team
B) A recommended medication dosage Claude calculated based on a patient's weight and age for use in a clinical setting
C) A plain-language explanation of how recursion works, requested by a student studying for a computer science course
D) An example CSV file structure Claude generated to illustrate proper comma-separated formatting for a tutorial

---

**Q10.** A legal operations team wants to use Claude to accelerate contract review. In their proposed workflow, Claude reads incoming vendor contracts, flags non-standard clauses, drafts a summary of risks, and then automatically approves contracts that score below a 'risk threshold' without any attorney review. As the solution designer, where is the critical flaw in this workflow?

A) Flagging clauses and drafting summaries are reasonable uses, but final approval decisions should not be automated based solely on Claude's output since it can miss nuance or hallucinate and carries legal/financial risk
B) Claude should not be used for contract review at all because it cannot read legal documents
C) The risk threshold scoring step should be removed entirely since Claude cannot produce numeric scores
D) The workflow is correct as designed because Claude's outputs are deterministic and repeatable for identical contracts

---

**Q11.** A procurement team currently has an analyst manually read 15-page supplier proposals, extract pricing terms, cross-reference them against a 3-page internal policy document, and write a one-paragraph recommendation. They want to redesign this as a Claude-assisted workflow. Which integration design BEST fits this use case?

A) Have Claude re-write the entire supplier proposal in simplified language before any human reads either document
B) Use Claude only to count the number of pages in the proposal so the analyst knows how long it will take to read
C) Skip Claude entirely and have the analyst continue manual review, since cross-referencing two documents exceeds what a single model call can handle
D) Send the full proposal and policy document together in a single prompt and ask Claude to extract terms, check them against policy, and draft the recommendation in one pass, with a human reviewing the output before it is sent

---

**Q12.** A customer support team is designing a Claude-assisted ticket workflow. Which pairing of task-to-automation-level is MOST appropriate?

A) Claude drafts a reply to a billing dispute AND automatically issues the refund if the draft mentions a dollar amount
B) Claude is given full autonomy to resolve all ticket types, including account closures, without agent review, since it reduces headcount costs
C) Claude categorizes incoming tickets by topic and drafts a suggested reply for the agent to review and send; a human agent independently approves any refund or account-level action
D) Claude is restricted to only replying 'please contact an agent' for every ticket, since support contains sensitive customer data

---

**Q13.** A team is building a workflow where Claude analyzes customer feedback transcripts and outputs a structured action plan that is then automatically pushed to a ticketing system. To reduce the risk of incorrect or hallucinated action items reaching the ticketing system, which design change is MOST effective?

A) Increase the length of the system prompt so Claude is told more firmly not to hallucinate
B) Run the same prompt twice and average the two outputs before pushing to the ticketing system
C) Insert a mandatory human review and approval step between Claude's output and the automatic push to the ticketing system
D) Remove structured output formatting so Claude can respond more naturally and reduce error rate

---

**Q14.** A market research team needs to synthesize findings across twelve long industry reports to answer a single strategic question. Which workflow design is generally preferable for this type of research task?

A) Paste all twelve full reports into a single prompt regardless of combined length and ask for one synthesized answer with no intermediate steps
B) Ask Claude to guess the answer based on the report titles alone to save processing time
C) Avoid using Claude for this task entirely, since synthesizing multiple documents is outside what the model can be used for
D) Have Claude summarize each report individually first, then synthesize the set of summaries into a final answer, reviewing intermediate summaries for accuracy along the way

---

**Q15.** When communicating Claude's limitations to a team that plans to use it for fact-based research summaries, which point is MOST important to convey?

A) Claude's confident and fluent writing style does not guarantee factual accuracy, so outputs used for research conclusions should be verified against sources, especially for specific facts, figures, or citations
B) Claude can never be used for research tasks and should be restricted to creative writing only
C) Claude's outputs are always 100% accurate as long as the prompt is phrased as a direct question
D) Claude's limitations only matter for coding tasks and are not relevant to research or writing tasks

---

**Q16.** A legal operations lead is designing a Claude-assisted contract workflow with four stages: (1) extracting key clauses and flagging unusual risk language from incoming contracts, (2) drafting redline suggestions against a standard playbook, (3) confirming the live, current signature status of a contract by checking the company's contract management database in real time, and (4) generating a plain-language risk summary for business stakeholders who are not lawyers. Which stage is the LEAST appropriate for Claude to handle without additional tooling, and why?

A) Stage 3, because Claude has no inherent real-time connection to external systems of record and cannot confirm current live data without being given tool access or an up-to-date data feed
B) Stage 1, because Claude cannot reliably read or parse unstructured legal text
C) Stage 4, because Claude cannot simplify technical language for non-expert audiences
D) Stage 2, because Claude cannot compare contract language against a reference playbook

---

**Q17.** A marketing analyst at a healthcare company wants to quickly summarize customer feedback that includes patient names, diagnoses, and insurance IDs. She plans to paste the raw feedback into her personal, free Claude.ai consumer account because it's the fastest option available. Per responsible AI and data-privacy practices, what is the BEST course of action?

A) Use the organization's approved enterprise Claude deployment (with a signed data processing agreement) and de-identify PHI before submission, per company policy
B) Proceed as planned, since Claude.ai conversations are never reviewed by anyone
C) Strip only the patient names before pasting, since diagnoses and insurance IDs are not considered sensitive health data
D) Paste the data into Claude.ai but switch on 'Incognito' mode to prevent any logging

---

**Q18.** A clinic is piloting Claude to help a nurse practitioner draft patient discharge instructions. Which practice aligns with Anthropic's Usage Policy for high-stakes domains like healthcare?

A) Use Claude only to generate a first draft, and require the licensed clinician to review and approve every draft before it reaches a patient
B) Allow Claude's draft to be sent to patients directly, since that saves clinician time
C) Fine-tune Claude on past discharge notes and disable any human review once accuracy exceeds 90% in internal testing
D) Restrict Claude to only non-clinical scheduling tasks, since the Usage Policy bans any involvement in clinical workflows

---

**Q19.** What is the primary purpose of Anthropic's Responsible Scaling Policy (RSP) and its associated AI Safety Levels (ASL)?

A) To establish technical and organizational safeguards that scale with a model's capability, triggering stricter controls as potentially dangerous capabilities are reached
B) To define pricing tiers for Claude API usage based on model capability
C) To set the maximum context window size allowed for each Claude model
D) To determine which customers are eligible for enterprise support contracts

---

**Q20.** A compliance officer asks whether prompts and outputs submitted through the Claude API will be used to train future Anthropic models. Which statement accurately reflects Anthropic's default commercial data policy?

A) All API data is automatically used to retrain Claude every 30 days unless the customer opts out
B) API data is permanently stored and used to train models unless the customer pays for an enterprise tier
C) Anthropic has no data retention policy, so API data is deleted instantly and never stored
D) By default, Anthropic does not use customer API prompts and outputs to train its models, and retains them only briefly for abuse monitoring unless an opt-in or legal exception applies

---

**Q21.** An HR team configures Claude to automatically reject job applicants who score below a threshold on an AI-generated 'culture fit' summary, with no human reviewing rejected applications. Which of the following represents the WORST practice among these options, per responsible-AI governance?

A) Using Claude to draft interview questions that a human recruiter then reviews and selects from
B) Using Claude to summarize a candidate's resume for a recruiter, who then makes the hiring decision
C) Using Claude to automatically reject candidates with no human review, risking undetected bias and unreviewable adverse employment decisions
D) Using Claude to check resumes for formatting errors before human review

---

**Q22.** A company publishes blog articles that are substantially written by Claude with minimal human editing, and does not disclose AI involvement to readers. From a responsible-AI governance standpoint, what is the main concern with this practice?

A) Claude-generated text is copyrighted by Anthropic, so publishing it without a license is illegal
B) Lack of transparency about AI-generated content can mislead readers and undermine trust, which many organizational AI policies and emerging regulations require disclosing
C) There is no concern, since Claude's outputs are always more factually accurate than human-written content
D) Claude cannot generate publishable long-form content, so this scenario is not technically feasible

---

**Q23.** A financial services employee needs an AI-generated summary of a report containing regulated customer PII (names, account numbers, balances). The firm's AI governance policy states regulated customer data may only be sent to a third-party AI system under a signed data processing agreement with contractual retention and confidentiality commitments, and explicitly notes that consumer-facing chat products do not meet this bar. Which action best complies with the policy?

A) Paste the full data into Claude.ai Free in a temporary chat and delete the conversation immediately after generating the summary
B) Process the data through the company's contracted Anthropic API deployment, which has a signed data processing agreement and retention configured to zero
C) Remove only the customer names from the records, then paste the remaining data into Claude.ai Pro to generate the summary
D) Ask a colleague to run the summary through their personal Claude Pro subscription since it uses the same underlying model

---

**Q24.** A knowledge worker needs Claude to analyze a 50-page legal contract and produce a structured risk summary with citations to specific clauses, so a lawyer can quickly verify each finding against the source text. Which approach BEST ensures accuracy and traceability?

A) Ask Claude to summarize the contract in one sentence per identified risk
B) Use a system prompt that simply tells Claude to be concise and accurate
C) Ask Claude to generate the summary without first being given the full document text
D) Instruct Claude to quote the exact clause text before each identified risk, using XML tags to separate the quoted text from the analysis

---

**Q25.** A team needs Claude to classify 500 customer support tickets into one of 5 fixed categories with perfectly consistent output formatting for downstream parsing. Which prompting technique is MOST effective for this requirement?

A) Multishot prompting with 3-5 labeled examples showing the exact ticket, reasoning (if any), and output format desired
B) Zero-shot prompting that simply lists the five category names in the instructions
C) Asking Claude to reason step-by-step through each ticket before stating a category
D) Running each ticket in a separate conversation with no examples provided

---

**Q26.** You need Claude's response to start directly with raw JSON output, with no preamble like 'Here is the JSON you requested:'. Which technique reliably achieves this?

A) Use prefilling by starting the Assistant turn with an opening character such as '{' so Claude continues directly from there
B) Add the word 'Please' to the beginning of the user prompt
C) Increase the temperature parameter to 1.0 to make output more direct
D) Add more negative instructions such as 'do not explain' repeated multiple times

---

**Q27.** A user wants Claude to produce a 20-page technical report requiring research synthesis, outline creation, section drafting, and final editing. Which task decomposition strategy is MOST effective for achieving high-quality output?

A) Give Claude the entire task in a single prompt and let it generate the whole report in one pass
B) Break the task into sequential prompts: first generate and approve an outline, then draft each section separately, then run a dedicated final editing pass
C) Ask Claude to write the full report twice and manually pick the better version
D) Instruct Claude to write the conclusion first, then work backwards to the introduction

---

**Q28.** What is the primary functional difference between placing instructions in the system prompt versus embedding them in the user turn when prompting Claude?

A) XML tags are only parsed correctly when placed in the system prompt, never in a user turn
B) The system prompt sets persistent role, context, and behavioral guidelines that apply across the whole conversation, while user turn instructions typically apply to that specific request
C) User turn instructions are always processed by Claude before the system prompt regardless of their order in the request
D) The system prompt cannot contain examples; only the user turn can include multishot examples

---

**Q29.** A Claude-generated draft is factually correct but uses a tone that's far too casual for the target executive audience. What is the MOST effective way to iterate on this output?

A) Start an entirely new conversation and write a much longer initial prompt
B) Lower the temperature setting and regenerate the response from scratch
C) Simply reply with 'try again' and let Claude infer what needs to change
D) Provide specific feedback identifying the tone problem, along with an example of the desired tone and a reference to the parts of the draft needing adjustment

---

**Q30.** A compliance team at a bank repeatedly asks Claude questions about an internal 80-page policy manual and three related procedure documents. They want these documents persistently available to every future conversation without re-uploading each time, and they want to update the documents centrally when policy changes occur. Which Claude product feature BEST meets these requirements?

A) Paste the full text of all documents into the system prompt of each new chat
B) Use research mode so Claude retrieves the policy information from the web each time
C) Create a Project and add the documents to its knowledge base
D) Generate an Artifact containing a summary of the documents for future reference

---

**Q31.** A product team wants Claude to generate an interactive, editable React dashboard component that updates live in a side panel as they iterate on the code with Claude, separate from the conversational explanation text. Which Claude feature is designed for this?

A) Projects
B) Research mode
C) Artifacts
D) Standard chat with code blocks

---

**Q32.** A startup runs an automated pipeline that classifies the sentiment of 5 million customer support tickets per day, where each classification is a short, simple task and the company's primary constraints are minimizing per-call latency and API cost. Which model is the BEST fit?

A) Claude Opus
B) Claude Sonnet
C) Claude Haiku
D) Whichever model has the largest context window

---

**Q33.** A researcher needs to analyze a 500,000-word legal archive that far exceeds any single Claude model's context window, and needs Claude's final answer to synthesize insights across the entire archive. What is the BEST approach?

A) Switch to Claude Opus and paste the entire archive into one prompt since Opus has the largest capacity
B) Use research mode so Claude can search the web for the archive's content instead of reading it directly
C) Truncate the archive to only the first 200,000 tokens and ignore the rest
D) Split the archive into sections, have Claude summarize or extract key points from each section, then synthesize those intermediate outputs into a final answer

---

**Q34.** A user asks Claude, 'What were the three most significant AI regulatory developments announced in the past two weeks across the US, EU, and UK?' Which approach is MOST appropriate for this request?

A) Standard chat with Claude Haiku, since the question is short and simple
B) Research mode, since the task requires current information gathered and synthesized from multiple live sources
C) A Project with a knowledge base of the company's internal policy documents
D) Generate an Artifact summarizing general AI regulation history

---

**Q35.** A team uploads a PDF of company policies to a Project's knowledge base. The policy is updated weekly on their internal wiki, but no one re-uploads a new file to the Project. When a user asks Claude about current policy a month later, what happens?

A) Claude automatically re-indexes the linked wiki source and reflects the latest policy because Project knowledge syncs continuously
B) Claude detects the staleness and automatically appends a disclaimer before answering
C) Claude continues referencing the outdated PDF content, because Project knowledge files are static snapshots that only update when manually re-uploaded
D) Claude merges the PDF with live wiki data automatically because connectors are enabled by default in every Project

---

**Q36.** A support team wants Claude to draft replies based on the most recent messages in a shared inbox that changes dozens of times per day. Which configuration approach best meets this requirement?

A) Connect the Gmail connector so Claude can retrieve live, current email content directly when needed
B) Export email threads and upload them to the Project knowledge base once per week
C) Paste the relevant emails into the chat manually each time a reply is needed
D) Write custom instructions describing the typical structure and tone of past emails

---

**Q37.** A Project has custom instructions stating 'always respond in a formal, professional tone,' but one of the uploaded knowledge documents contains example replies written in a casual, conversational style. When generating a response, how does Claude typically resolve this conflict?

A) Claude treats the casual examples in the knowledge document as an override since knowledge content is more specific than general instructions
B) Claude ignores both and defaults to its base model tone without reconciling the conflict
C) Claude prioritizes the custom instructions as explicit behavioral directives, treating the knowledge document's content as reference material rather than a style directive
D) Claude alternates between tones across responses to balance both sources equally

---

**Q38.** What is the key distinction between Project-level custom instructions and settings applied only within a single conversation in Claude.ai?

A) Project custom instructions apply only to the first message of a conversation, while in-chat settings apply to every message
B) There is no functional difference; both terms describe the same configuration mechanism
C) Project custom instructions can only be configured by a workspace owner and never by an individual Project member
D) Project custom instructions persist across every conversation created within that Project, while single-conversation settings affect only that one chat

---

**Q39.** An Enterprise admin disables the Google Drive connector at the organization level after several users had already connected their personal Google Drive within individual Projects. What is the expected result for those existing connections?

A) Existing connections keep working but require reauthorization every 24 hours
B) Existing Project connections continue functioning, but no new Google Drive connections can be created by anyone in the organization
C) Only newly created Projects are affected; Projects that existed before the admin change retain connector access permanently
D) Access through the connector is revoked for all users immediately, since the organization-level setting overrides individual user-level connector authorizations

---

**Q40.** A team's RAG workflow sends Claude a prompt in this exact order: (1) detailed instructions describing how to extract clauses, (2) a 150,000-token internal contract, with no restatement of the question after the document. Claude frequently misses clauses located in the middle of the contract, even though the full document fits comfortably within the model's context window. Which change is BEST for improving extraction accuracy?

A) Add the instructions a second time, keeping them before the document, so Claude reads them twice
B) Break the document into 10 separate API calls of 15,000 tokens each and merge the results
C) Reduce the document size by summarizing it with Claude before running the extraction prompt
D) Move the detailed instructions and question to appear AFTER the document instead of before it

---

**Q41.** A developer asks Claude to respond with raw JSON only, but Claude consistently prepends a sentence like "Here is the JSON output you requested:" before the object, breaking an automated parser. The system prompt already states "Respond only with valid JSON, no other text." Which technique is MOST effective at reliably eliminating the preamble?

A) Prefill the start of Claude's response (the Assistant turn) with an opening character like "{"
B) Lower the temperature to 0 so Claude becomes more deterministic
C) Increase max_tokens so Claude has more room to finish its explanation before the JSON
D) Add the word "IMPORTANT" in all caps before the instruction in the system prompt

---

**Q42.** A QA team is building an automated regression suite that calls Claude with the same prompt repeatedly and expects the output to be nearly identical across runs, so they can catch regressions whenever the prompt is modified. Which configuration adjustment BEST supports this goal?

A) Set top_p to 1.0 and temperature to 1.0 for maximum consistency
B) Enable extended thinking mode to make Claude reason more carefully before each response
C) Increase max_tokens to ensure Claude never truncates the response differently between runs
D) Set temperature close to 0 (e.g., 0) to minimize output variability

---

**Q43.** Claude's response to a summarization prompt is being cut off mid-sentence in production, even though the prompt and context length are well within the model's documented context window. Which single parameter adjustment is the DIRECT fix for this specific symptom?

A) Add a stop_sequence that matches common sentence-ending punctuation
B) Decrease the temperature parameter to improve fluency
C) Increase the max_tokens parameter in the API request
D) Switch to a model with a larger context window

---

**Q44.** A team notices their production prompt performed well on the handful of examples they tested manually during development, but it fails unpredictably on a wider variety of real user inputs after launch. Which practice would have MOST effectively caught this issue before launch?

A) Writing a longer, more detailed system prompt with more explicit instructions
B) Building a diverse evaluation dataset of representative test cases and systematically measuring output quality across all of them before deployment
C) Increasing the temperature during development to see a wider range of possible outputs
D) Asking Claude to self-critique its own response immediately after generating it

---

