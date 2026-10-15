# AI for Business Workflows — lesson evidence audit

**Audit date:** 15 October 2026  
**Status:** Source-mapped — review in progress; not independently peer-reviewed.

## Lesson-level source map

| Lesson | Key claims / objective | Primary reading | Limits and review notes |
|---|---|---|---|
| Choose the Right Task for AI | Define task, users, risks, success criteria and oversight before automation. | NIST AI RMF resources: https://www.nist.gov/itl/ai-risk-management-framework/ai-risk-management-framework-resources; NIST Generative AI Profile: https://doi.org/10.6028/NIST.AI.600-1 | NIST frameworks are voluntary risk-management guidance, not automatically legal requirements. Risk depends on use case and context. |
| Write Clear Instructions and Prompts | Specify task, context, constraints, format, quality criteria and uncertainty rules. | OpenAI prompt engineering guide (vendor guidance): https://platform.openai.com/docs/guides/prompt-engineering; NIST AI RMF resources: https://www.nist.gov/itl/ai-risk-management-framework/ai-risk-management-framework-resources | Vendor documentation is practical guidance, not independent empirical evidence. The example prompt is original. |
| Map the Workflow and Human Handoffs | Define triggers, inputs, validation, approvals, actions and logs. | NIST AI RMF 1.0: https://doi.org/10.6028/NIST.AI.100-1; NIST Generative AI Profile: https://doi.org/10.6028/NIST.AI.600-1 | The workflow is an original practical template. Meaningful oversight requires authority, time and expertise, not merely a human checkbox. |
| Evaluate Accuracy, Bias and Reliability | Build test sets, define criteria, track failures, verify evidence and monitor changes. | NIST AI RMF 1.0: https://doi.org/10.6028/NIST.AI.100-1; NIST Generative AI Profile: https://doi.org/10.6028/NIST.AI.600-1 | Avoid claims that a single benchmark guarantees safety or general performance. Evaluation needs task-specific test data and ongoing monitoring. |
| Protect Data and Launch Responsibly | Minimise data, restrict permissions, assign ownership and define incident/stop processes. | NIST AI RMF resources: https://www.nist.gov/itl/ai-risk-management-framework/ai-risk-management-framework-resources; NIST Generative AI Profile: https://doi.org/10.6028/NIST.AI.600-1 | Privacy, security and legal obligations vary by jurisdiction and data type. NIST guidance does not replace legal review. |

## Knowledge check review
- Task definition question: answer 2.
- Confidence and accuracy question: answer 3.
- Safer prototype question: answer 2.
- Explanations align with the lessons and emphasise verification, limited testing and human review. The three-item quiz is not a validated AI safety assessment.

## Publication gate
Clearly distinguish standards guidance from law and vendor documentation from independent research. Do not imply AI output is reliable merely because it is fluent. Keep the course labelled **source-mapped — review in progress**.

**Reviewer:** automated editorial/source-mapping pass; no independent AI governance or legal review recorded.  
**Open work:** map each claim to exact NIST section numbers; test examples on representative cases; check data-protection and sector-specific requirements for the intended jurisdictions; review assessment and source reuse terms.


## Source inspection log — 15 October 2026

### Direct sources inspected
- **NIST AI RMF 1.0**, NIST AI 100-1, official PDF: https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-1.pdf. The framework describes four functions—GOVERN, MAP, MEASURE and MANAGE—and positions governance across the AI lifecycle. Its measures include testing before deployment and regularly during operation. This supports the course's lifecycle, risk-owner and monitoring themes; it does not establish that a particular workflow is safe merely because a checklist is completed.
- **NIST Generative AI Profile**, NIST AI 600-1, official PDF: https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.600-1.pdf. It is a cross-sectoral companion profile for generative AI and proposes risk-management actions across the lifecycle. It is guidance, not a substitute for use-case-specific validation or applicable law.
- **NIST AI RMF Core**, official section page: https://airc.nist.gov/airmf-resources/airmf/5-sec-core/. It explains that the four functions are divided into categories and subcategories and that the actions are not a rigid checklist or necessarily ordered steps.
- **OpenAI prompt engineering guide**, official vendor documentation: https://developers.openai.com/api/docs/guides/prompt-engineering. It recommends representative prompt tests/evaluation suites and notes output non-determinism and model-version differences. This is vendor guidance, not independent empirical evidence; the course should not imply a single prompt template guarantees accuracy.

### Claim-level review and limitations
- The course's task definition, iterative evaluation, human approval, and monitoring principles are consistent with the inspected frameworks at a high level.
- The course's six-part prompt structure is an original teaching template, not a standard or empirically proven universal formula.
- “High-impact decisions” is deliberately broad and should be supplemented with jurisdiction- and sector-specific examples before publication for a particular market.
- The quiz key remains internally consistent: question 1 answer index 1, question 2 answer index 2, question 3 answer index 1. This is a small formative check, not a validated competency assessment.
- No individual peer-reviewed empirical study was inspected in this pass. This course is principally an applied framework-based introduction, not a research review.
- No legal/privacy counsel review, independent AI-governance SME review, live browser interaction test, or full production deployment test was performed.

### Remaining publication gate
Keep the status **source-mapped — review in progress**. Before claiming “verified” or “research-backed,” map important claims to exact NIST sections, test the practical workflow on representative examples, review local data-protection and sector rules, inspect source reuse terms, and obtain independent subject-matter and assessment review.
