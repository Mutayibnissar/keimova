# Business Analytics Essentials — lesson evidence audit

**Audit date:** 15 October 2026  
**Status:** Source-mapped — review in progress; not independently peer-reviewed.

## Lesson-level source map

| Lesson | Key claims / objective | Reading inspected or assigned | Limits and review notes |
|---|---|---|---|
| Start with a Business Question | Define a decision, population, time period and what evidence could change an action. | OpenIntro Statistics, official textbook and course resources: https://www.openintro.org/book/os/ | The question-first routine and four analytics labels are teaching frameworks, not a claim that every organisation uses one universal taxonomy. Source is a textbook landing/resource page; exact chapter-level review remains open. |
| Data Quality Before Analysis | Check missing values, duplicates, row definitions, units, authorisation and privacy. | NIST Privacy Framework: https://www.nist.gov/privacy-framework; OpenIntro Statistics: https://www.openintro.org/book/os/ | NIST describes a voluntary enterprise-risk framework for managing privacy risk; it does not replace applicable law or an organisation's policy. Missing data treatment depends on context; do not automatically replace missing values with zero. |
| Descriptive Statistics and Segmentation | Interpret mean, median, rates and group comparisons. | OpenIntro Statistics, Chapter 2: Summarizing Data resources: https://www.openintro.org/book/os/ | Official OpenIntro site lists Chapter 2 resources for summarizing data. Exact chapter text and licensing/reuse terms should be checked before adapting material. Example arithmetic checked independently: values ₹100, ₹120, ₹130, ₹150 and ₹1,000 sum to ₹1,500; mean ₹300; median ₹130. Neither statistic is universally best. |
| KPIs, Funnels and Trends | Define metric numerator/denominator; calculate rates and avoid causal overclaiming. | OpenIntro Statistics resources: https://www.openintro.org/book/os/; OpenStax, *Introductory Business Statistics 2e*, §13.4: https://openstax.org/books/introductory-business-statistics-2e/pages/13-4-the-regression-equation | The inspected OpenStax regression section explains model assumptions and limitations. It is not a dedicated source for KPI design or funnel analytics; those topics remain practical teaching guidance. 100/2,000 = 5%; 20/100 = 20%. Fictional examples only. |
| SQL Thinking and Communicating Insights | Explain SELECT/FROM/WHERE/GROUP BY and communicate findings with limitations. | SQLBolt Lesson 1: https://sqlbolt.com/lesson/select_queries_introduction; Lesson 2: https://sqlbolt.com/lesson/select_queries_with_constraints; Lesson 10: https://sqlbolt.com/lesson/select_queries_with_aggregates; Lesson 11: https://sqlbolt.com/lesson/select_queries_with_aggregates_pt_2 | SQLBolt is an interactive learning resource, not scholarly research. Lesson 10 explicitly describes aggregate functions and grouped summaries; Lesson 11 covers HAVING after grouping. Test the example query against a defined sample schema before claiming it runs in a specific database. |

## Source inspection log

### NIST Privacy Framework
The official NIST page describes the Privacy Framework as a **voluntary** tool for identifying and managing privacy risk through enterprise risk management. Its functions include Identify-P, Govern-P, Control-P, Communicate-P and Protect-P. This supports the course's general emphasis on privacy risk and governance, but not a blanket legal-compliance claim. See: https://www.nist.gov/privacy-framework and https://www.nist.gov/privacy-framework/frequently-asked-questions.

### OpenStax regression section
The official *Introductory Business Statistics 2e* section 13.4 presents the linear regression equation and discusses assumptions including error behaviour, variance and independence. It also explains that violated assumptions affect estimate quality. This is relevant background for caution around modelling, but it is not evidence that correlation establishes causation; the course correctly cautions against making that inference. Source inspected: https://openstax.org/books/introductory-business-statistics-2e/pages/13-4-the-regression-equation.

### SQLBolt lessons 10–11
The official interactive lessons describe aggregate functions including COUNT, MIN, MAX, AVG and SUM, and show how GROUP BY summarizes records into groups. Lesson 11 explains HAVING as a condition applied to grouped rows. This supports the basic SQL concepts in the lesson. Sources inspected: https://sqlbolt.com/lesson/select_queries_with_aggregates and https://sqlbolt.com/lesson/select_queries_with_aggregates_pt_2.

### OpenIntro Statistics
The official OpenIntro site describes the book as an introductory college statistics text and lists Chapter 2 resources on summarizing data. The textbook is assigned as further reading, but this audit has **not** recorded a page-by-page inspection of the full chapter. No claims are made here that individual empirical papers were inspected or that the course has been peer-reviewed. Source: https://www.openintro.org/book/os/ and https://www.openintro.org/book/os/pdf/.

## Knowledge check review
- First-step question: answer B (index 1).
- Missing-value question: answer False (index 1).
- Rate question: answer B (index 1); 100/2,000 = 5%.
- Answer keys and arithmetic are internally consistent. The three-item quiz is not a validated assessment.

## Publication gate
Separate calculation correctness from interpretation quality. Keep simulated examples labelled, document dataset assumptions and privacy controls, and avoid treating correlation as causation. Do not call the course “verified”, “peer-reviewed” or “research-backed” solely because it has reading links.

**Reviewer:** automated editorial/source-mapping pass; no independent statistics/data-protection expert review recorded.  
**Open work:** inspect the relevant OpenIntro chapter text and reuse/license terms; add dedicated sources for experimental design/causal inference if taught in depth; test SQL against a defined schema; review privacy wording for target jurisdictions; perform browser-level interaction tests.
