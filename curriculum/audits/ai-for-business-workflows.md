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
