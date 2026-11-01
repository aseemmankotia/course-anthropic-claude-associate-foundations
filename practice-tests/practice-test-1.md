# Practice Test 1: CCAO-F: Claude Certified Associate Foundations Exam Prep

- **Questions:** 44
- **Time limit:** 90 minutes
- **Passing score:** 70%%

> Answers are in `answer-key-1.md`. Track results in `score-tracker.md`.

---

**Q1.** A paralegal asks Claude to summarize a contract dispute and cite relevant case law. Claude responds confidently with a summary and references 'Harrison v. Meridian Trust (2019)' including a specific docket number. The paralegal has never heard of this case. What is the BEST next step?

A) Accept the citation because Claude's confident, detailed tone indicates accuracy
B) Ask Claude to rephrase the citation more cautiously, then accept it
C) Reject the entire summary since any single unverifiable detail invalidates all of Claude's output
D) Independently search a legal database to verify the case exists and matches the cited facts before using it

---

**Q2.** A developer needs Claude's output to be automatically parsed by a downstream Python script with zero manual cleanup. Which approach to formatting the request is BEST?

A) Ask Claude to respond only with valid JSON matching a specific schema, and instruct it to return no extra commentary outside the JSON
B) Ask Claude to 'explain the results clearly' and parse the prose with regex
C) Ask Claude to use a numbered list so the script can split on line breaks
D) Ask Claude to format the answer as a Markdown table for readability

---

**Q3.** A user asks Claude to suggest a likely diagnosis based on a list of symptoms, and Claude provides a clear, well-reasoned answer with appropriate caveats. What is the correct handling of this output before any action is taken?

A) Act on the suggestion directly since Claude included appropriate medical caveats
B) Re-prompt Claude three times and accept the diagnosis only if all three answers agree
C) Route the output to a licensed medical professional for review before any clinical decision is made, regardless of how confident or well-caveated the response is
D) Accept the output as valid since Claude is trained on extensive medical literature

---

**Q4.** Which of the following is the MOST reliable indicator that a Claude response may contain a hallucination?

A) The response is phrased in a confident, assertive tone
B) The response includes highly specific facts (exact dates, statistics, or citations) that cannot be independently corroborated against a trusted source
C) The response is long and detailed
D) The response uses complex vocabulary and technical terminology

---

**Q5.** A team wants to evaluate whether Claude's hiring-recommendation outputs show demographic bias. Which testing method BEST detects this?

A) Ask Claude directly whether its output is biased and accept its self-assessment
B) Read the output once and judge subjectively whether it 'feels' fair
C) Submit the same resume and prompt multiple times with only the candidate's name/gender/ethnicity cues varied, then compare the outputs for systematic differences
D) Check if the output uses polite, professional language throughout

---

**Q6.** A user submits a prompt containing five distinct sub-questions. Claude's response thoroughly answers four of them but silently omits the fifth. Before treating this output as complete, what should the reviewer do?

A) Assume the fifth question was unanswerable and move on
B) Accept the response as complete since four out of five is a strong response rate
C) Submit the exact same prompt again and expect Claude to self-correct automatically
D) Notice the omission, and either re-prompt Claude to address the missing sub-question or manually verify why it was skipped before considering the task done

---

**Q7.** A legal team uses Claude to summarize incoming contracts and extract key dates, dollar amounts, and obligations, which are then dropped into an email sent directly to the client. Which practice BEST ensures the output is reliable before it reaches the client?

A) Send Claude's summary as-is, since it quotes language directly from the contract
B) Increase the model's temperature setting so the extracted details are more creative and complete
C) Have a human compare every extracted date, dollar amount, and obligation against the source contract before the email is sent
D) Add a generic disclaimer to the email stating the summary was AI-generated, with no further review

---

**Q8.** A team is building a pipeline where Claude extracts product attributes (name, price, SKU, category) from supplier emails and the result is immediately ingested into a database by a downstream script. Which output format should be requested to minimize parsing errors and support automated validation?

A) JSON output that strictly conforms to a predefined schema
B) A freeform paragraph summarizing the product details in natural language
C) A markdown table with one column per attribute
D) A bulleted list with attributes written in varying order per item

---

**Q9.** Claude responds to a research question with a confident citation: "According to Smith et al. (2021), p. 47, adoption rates increased 34%." The user has no prior familiarity with this paper. What is the appropriate verification step before relying on this citation?

A) Trust the citation because it includes a specific author, year, and page number
B) Ask Claude to restate the citation in a different format to confirm it is correct
C) Accept the claim since the model's confident, detailed tone indicates high reliability
D) Independently locate and check the actual source to confirm the paper, page, and statistic exist and match

---

**Q10.** A financial analyst's workflow includes: (1) extracting data points from quarterly earnings PDFs, (2) summarizing key financial trends from the extracted data, (3) drafting a narrative analysis for stakeholders, and (4) finalizing the official investment recommendation sent to clients. Which step requires a human to retain final accountability, making it the LEAST appropriate for Claude to complete independently?

A) Step 2 - summarizing financial trends from provided data
B) Step 1 - extracting data points from earnings PDFs for initial review
C) Step 4 - finalizing the official investment recommendation sent to clients
D) Step 3 - drafting the narrative analysis

---

**Q11.** A marketing team runs a recurring weekly workflow: they want Claude to automatically have access to the same brand guidelines and past campaign examples every session, without re-uploading them each time. Which Claude.ai feature should they use?

A) Export and manually paste previous chat history into each new conversation
B) Start a new standalone chat each week and manually attach the files
C) Use the API with only a system prompt and no file handling
D) Use a Project with the guidelines and examples added as Project knowledge

---

**Q12.** Within a Claude.ai Project, a team wants every new conversation to automatically start with an instruction that Claude always respond using a specific JSON schema for downstream automation, without repeating the instruction manually each time. Which Project configuration should they use?

A) Claude's unmodified default system prompt
B) Project-level custom instructions
C) Project knowledge files
D) Individual saved chat templates pasted into each new chat

---

**Q13.** A customer support team is evaluating Claude for ticket handling, which includes: categorizing incoming tickets by topic, drafting first-response replies to common questions, and approving refunds above $500 that fall outside standard policy. Leadership asks where Claude should NOT operate autonomously. What is the BEST answer?

A) Categorizing tickets by topic, since this requires contextual judgment
B) All three tasks are equally safe to fully automate
C) Approving refunds above $500 that fall outside standard policy, since this involves exception-based judgment and financial accountability
D) Drafting first-response replies to common questions, since tone matters

---

**Q14.** A research analyst asks Claude for today's stock price and a regulatory ruling issued this morning, in a session where tool use or web search has not been enabled. What is the MOST accurate limitation the team should communicate about this use case?

A) Claude can always access the internet in real time by default in every deployment
B) Claude's context window prevents it from processing any numerical data
C) Claude's training data has a knowledge cutoff, so without tool use or search enabled it cannot reliably provide live or very recent information
D) Claude will always refuse to respond at all when asked about recent events

---

**Q15.** When communicating Claude's value and limitations to a non-technical team adopting it for a research-heavy workflow, which statement BEST frames an appropriate expectation?

A) Claude can significantly accelerate drafting, synthesis, and brainstorming, but outputs on factual or high-stakes claims should still be verified before use
B) Claude's outputs are guaranteed to be free of bias or error
C) Claude eliminates the need for fact-checking entirely since it is always accurate
D) Claude should only be used for tasks that require absolutely no human review at any stage

---

**Q16.** A legal operations team wants to integrate Claude into their contract review workflow, which includes: (1) extracting key clauses from contracts, (2) summarizing obligations for each party, and (3) issuing final legal risk sign-off before contract execution. Which approach BEST reflects where Claude should and shouldn't be used in this workflow?

A) Use Claude to extract clauses and draft obligation summaries to accelerate the review, but require a qualified human to make the final legal risk sign-off decision
B) Use Claude for all three steps, including final sign-off, since it can analyze legal risk comprehensively and consistently
C) Avoid using Claude entirely for this workflow since legal documents are too sensitive to involve an AI model
D) Use Claude only for the final sign-off step since it is the most time-consuming, and have humans perform extraction and summarization manually

---

**Q17.** An HR analyst wants to paste a batch of employee performance reviews containing full names, salaries, and medical leave details into Claude.ai (consumer version) to get a summary for an internal report. According to responsible AI practices, what is the BEST course of action?

A) Proceed as normal since Claude.ai conversations are never used for any purpose beyond answering the request
B) Redact or anonymize the names, salaries, and medical details before submitting, or use an enterprise offering with appropriate data handling terms
C) Split the data into smaller batches so no single prompt contains too much sensitive information
D) Convert the data to a PDF first, since file uploads are treated differently from pasted text for privacy purposes

---

**Q18.** A marketing team wants to use Claude to draft a product safety warning label for a medical device. The output will be used as-is without review by a qualified safety or legal professional. Is this an appropriate use case?

A) Yes, because Claude's training includes extensive medical and regulatory content
B) Yes, as long as the prompt explicitly asks Claude to be accurate and cite sources
C) No, because Claude cannot generate any text related to medical topics
D) No, because high-stakes safety-critical content requires human expert review before use, regardless of draft quality

---

**Q19.** An employee discovers that their organization's internal AI usage policy prohibits submitting customer contract text to any third-party AI tool. They believe using Claude would significantly speed up contract review. What should they do?

A) Use Claude anyway since the time savings outweigh the policy risk
B) Submit only short excerpts of the contracts so the full agreement is never exposed at once
C) Follow the organizational policy and raise the request with the appropriate team to evaluate an approved, compliant solution
D) Use a personal Claude account instead of a work account to avoid violating company IT policy

---

**Q20.** A company needs an AI solution to summarize internal legal documents containing privileged attorney-client information, and requires contractual guarantees about data handling, retention, and training-data exclusion. Which approach BEST meets these requirements?

A) Claude.ai Free tier, since all tiers follow the same consumer data policy
B) An enterprise agreement with Anthropic (e.g., Claude for Enterprise/API with a business agreement) that includes defined data handling and retention terms
C) Claude.ai Pro, configured with a strong system prompt instructing it to keep data private
D) Any Claude access method, since Anthropic never uses customer data for training regardless of agreement type

---

**Q21.** Before deploying a Claude-powered chatbot to answer customer questions about loan eligibility, which configuration step is MOST important from a responsible-use standpoint?

A) Maximizing the temperature setting so responses sound more natural and varied
B) Establishing a human escalation path and review process for eligibility decisions, since these have significant financial impact on customers
C) Disabling all logging so customer conversations cannot be reviewed later
D) Giving the chatbot a friendly persona name to build customer trust

---

**Q22.** Which statement BEST describes why diverse and representative review of AI-generated outputs matters in a responsible-use program?

A) It helps identify biased, unfair, or harmful outputs that a narrow reviewer group might miss or consider normal
B) It is only necessary for outputs generated in languages other than English
C) It is required solely to satisfy marketing claims about inclusivity
D) It eliminates the need for any other AI governance controls, such as data handling policies

---

**Q23.** An employee needs help from Claude drafting a reply to a customer complaint. The complaint email includes the customer's full name, home address, and credit card number. According to standard responsible-AI data handling practices, what should the employee do before submitting the request to Claude?

A) Redact or anonymize the sensitive personal and financial details before submitting the request
B) Submit the full complaint text as-is so Claude has complete context for the most accurate response
C) Replace the credit card number with its SHA-256 hash value and submit the rest of the complaint unchanged
D) Submit the request through a different Claude model variant that offers stronger privacy guarantees

---

**Q24.** A paralegal needs Claude to extract all parties, obligations, and deadlines from a 50-page contract into a structured table for review. Which prompting approach is BEST for this task?

A) Provide a single prompt with an explicit output schema (e.g., XML tags for <party>, <obligation>, <deadline>) and instructions to extract each category systematically
B) Ask Claude to "summarize this contract" with no additional instructions, then manually reformat the output into a table afterward
C) Ask Claude to "read the contract carefully and tell me what's important"
D) Upload the contract and ask Claude open-ended questions one at a time about whatever seems relevant

---

**Q25.** A developer wants Claude to write a Python function, test it against sample inputs, and fix any bugs found — all within one working session. Which prompting strategy best supports this iterative workflow?

A) Write a single prompt asking Claude to "write perfect, bug-free code" on the first attempt
B) Ask Claude to write five different implementations and pick the best one without testing any of them
C) Decompose the task into sequential turns: first generate the function, then ask Claude to test it against sample inputs and report results, then ask it to fix any issues found before finalizing
D) Provide the function requirements once and tell Claude not to respond until it is 100% certain the code is correct

---

**Q26.** You need Claude to solve a multi-step word problem involving several conditional calculations, and you want to minimize arithmetic errors. Which technique should you use?

A) Repeat the same prompt multiple times and average the numeric answers given
B) Ask for the final numeric answer only, with no explanation, to keep the response short
C) Ask Claude to answer in a single word to reduce token usage
D) Instruct Claude to work through the problem step-by-step (e.g., inside <thinking> tags) before stating the final answer

---

**Q27.** You need Claude's response to be strictly valid JSON with no leading explanation or trailing commentary, so it can be parsed directly by a downstream script. Which approach BEST ensures this?

A) Increase the temperature parameter so Claude is more creative and less repetitive in formatting
B) Specify the exact JSON schema in the prompt, instruct Claude to output ONLY the JSON object, and prefill the start of the assistant turn with "{" to constrain the response format
C) Ask Claude to write the JSON and then separately ask it to remove any extra text in a follow-up turn
D) Ask Claude nicely to "please only output JSON" and trust it will comply every time

---

**Q28.** A team is using the API for two different tasks: (1) extracting exact dates from invoices and (2) brainstorming multiple creative taglines for an ad campaign. How should they configure the temperature parameter for each task?

A) Temperature has no meaningful effect on Claude's output and can be ignored
B) Use a high temperature (close to 1) for both tasks to maximize output diversity
C) Use a low temperature (near 0) for both tasks to ensure consistency
D) Use a low temperature (near 0) for date extraction, and a higher temperature for tagline brainstorming to encourage varied, creative outputs

---

**Q29.** In the context of prompting Claude for complex, multi-part tasks, what does "task decomposition" refer to?

A) Breaking a complex task into smaller, sequential subtasks that can each be completed and verified before moving to the next
B) Lowering the temperature parameter to simplify Claude's reasoning process
C) Asking Claude multiple unrelated questions in a single prompt to save time
D) Reducing the length of the prompt by removing all context and instructions

---

**Q30.** A company needs to classify 50,000 short customer support tickets per day into categories, prioritizing low cost and fast response time over deep reasoning. Which Claude model BEST meets these requirements?

A) Claude Opus — highest capability model, but highest cost and latency, unnecessary for simple ticket classification
B) Claude Haiku — fastest and most cost-effective model, well-suited for high-volume, low-complexity classification tasks
C) Claude Sonnet — balanced performance and cost, but more expensive than needed for simple categorization at this volume
D) Claude Opus accessed through a Project with custom instructions — adds unnecessary setup and cost for this task

---

**Q31.** A research team needs Claude to search the web across multiple sources, synthesize findings, and produce a cited report answering a complex open-ended question that requires several rounds of investigation. Which Claude product capability BEST fits this need?

A) Artifacts — renders standalone outputs like code or documents in a side panel but does not perform iterative research
B) Research mode — performs iterative web searches and synthesizes multi-source findings into a cited report
C) Standard chat — a single-turn conversational interface without built-in multi-step web search orchestration
D) Projects — organizes related conversations and shared files but does not independently search the web

---

**Q32.** A developer asks Claude to generate a standalone HTML/CSS/JS prototype that updates live and can be viewed separately from the chat transcript as the developer iterates on it. Which Claude.ai feature is designed for this workflow?

A) Chat — the default conversational interface without a dedicated preview panel
B) Research mode — focused on multi-source web synthesis, not code generation or preview
C) Projects — organizes files and context across conversations but does not provide a live preview panel
D) Artifacts — displays generated content such as code, documents, or diagrams in a dedicated, iteratively editable panel

---

**Q33.** A product team wants to give Claude persistent access to their style guide, API documentation, and prior reference material so every new conversation starts with shared context, without re-uploading files each time. Which Claude feature should they use?

A) Research mode — oriented toward ad hoc web research tasks, not persistent internal knowledge storage
B) Artifacts — generates and displays standalone outputs but does not retain shared context across sessions
C) Standard chat — each conversation is independent and does not retain uploaded files from other chats
D) Projects — lets teams upload reference files and set custom instructions that persist across all conversations within the project

---

**Q34.** By default, what context window size do the Claude 3 family models (Haiku, Sonnet, and Opus) support?

A) 32,000 tokens
B) 200,000 tokens
C) 100,000 tokens
D) 1,000,000 tokens

---

**Q35.** A legal team creates a Claude Project and wants every chat within it to automatically follow a specific citation style, formal tone, and response length — without anyone needing to repeat these instructions in each conversation. Which configuration should they use?

A) Upload a style guide document to Project Knowledge
B) Ask each team member to paste the style guide into their first message
C) Set Custom Instructions at the Project level
D) Connect Google Drive and link the style guide file

---

**Q36.** A sales team's Claude Project needs to reference their team's shared Google Docs, which are edited and updated multiple times per week. Which setup requires the LEAST ongoing manual maintenance to keep Claude's responses current?

A) Connect the Google Drive connector so Claude can access the live documents
B) Re-upload updated copies of the docs to Project Knowledge each week
C) Paste the full document text into the Custom Instructions field
D) Create a brand-new Project every time a document changes

---

**Q37.** An admin keeps trying to add new reference files to a Project's Knowledge, but the interface indicates the Project Knowledge capacity has been reached. What must the admin do to add the new files?

A) Remove or replace some existing files in Project Knowledge to free up space
B) Wait 24 hours for the capacity to automatically reset
C) Switch the Project's custom instructions to a shorter version
D) Disconnect any connected integrations like Google Drive or Gmail

---

**Q38.** Within a Claude Project, what is the key functional difference between Custom Instructions and Project Knowledge?

A) Custom Instructions store reference documents, while Project Knowledge controls Claude's tone and behavior
B) They serve the exact same purpose and can be used interchangeably
C) Custom Instructions shape how Claude responds, while Project Knowledge supplies reference content Claude can draw facts from
D) Custom Instructions only apply to connectors, while Project Knowledge only applies to uploaded files

---

**Q39.** Several months after connecting Gmail to a support team's Claude Project, an admin notices Claude is referencing outdated email threads that no longer reflect current policies, confusing responses. What is the BEST action to maintain the Project's configuration going forward?

A) Permanently disconnect Gmail so Claude never accesses email again
B) Create a duplicate Project each quarter instead of maintaining the existing one
C) Periodically review the connector's scope and remove or update outdated Project Knowledge content so the configuration stays current
D) Ignore the issue since Claude will automatically disregard old information

---

**Q40.** A support-ticket summarization prompt produces summaries that vary wildly in structure and length across different runs, even though the input tickets are similar in format. Which change is MOST likely to fix this inconsistency?

A) Increase the temperature parameter so Claude has more flexibility to choose wording
B) Add a concrete example of the desired summary wrapped in XML tags so Claude has a template to follow
C) Remove the system prompt entirely so Claude isn't constrained by prior instructions
D) Switch to streaming responses so output arrives faster and feels more consistent

---

**Q41.** A retrieval-augmented generation (RAG) assistant occasionally states facts that do not appear anywhere in the retrieved documents provided in the prompt. Which prompt adjustment BEST addresses this?

A) Explicitly instruct Claude to answer only using the provided context and to say it doesn't know if the answer isn't present
B) Lower the max_tokens parameter so Claude has less room to add extra content
C) Prefill the response with the word 'Based' to force a factual tone
D) Increase the temperature so Claude is less repetitive in its phrasing

---

**Q42.** A team's prompt performs well in manual testing but starts failing on edge cases discovered after production deployment. Before rolling out any prompt changes, they want to systematically test revised prompt versions against a representative set of saved inputs and expected outputs. Which Anthropic Console feature is designed for this?

A) The Message Batches API
B) The Workbench chat interface
C) The Model Comparison page
D) The Evaluate tool

---

**Q43.** A production workflow performs simple binary classification (spam vs. not-spam) using Claude Opus 4.5 with a lengthy system prompt. Latency and per-call cost are higher than the team wants, but accuracy is already sufficient. Which single change would MOST improve cost and latency while keeping accuracy acceptable for this straightforward task?

A) Enable extended thinking so Claude reasons more carefully before answering
B) Switch the workflow to a smaller, faster model such as Claude Haiku
C) Add ten additional few-shot examples to reinforce the classification pattern
D) Increase the temperature to help Claude respond more quickly

---

**Q44.** When troubleshooting a prompt that is producing poor results, what is the recommended best practice for isolating the root cause of the problem?

A) Rewrite the entire prompt from scratch on every iteration to avoid carrying over flawed assumptions
B) Switch to a different model family on each test run to see which one performs best
C) Raise the temperature on each attempt to introduce more variety into the responses
D) Change one element of the prompt at a time and re-evaluate before making further changes

---

