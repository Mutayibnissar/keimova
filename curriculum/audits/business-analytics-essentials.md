# Business Analytics Essentials — lesson evidence audit

**Audit date:** 15 October 2026  
**Status:** Source-mapped — review in progress; not independently peer-reviewed.

## Lesson-level source map

| Lesson | Key claims / objective | Primary reading | Limits and review notes |
|---|---|---|---|
| Start with a Business Question | Define the decision, population, time period and what evidence would change an action. | OpenStax, *Introductory Business Statistics*, definitions and key terms: https://openstax.org/books/introductory-business-statistics/pages/1-1-definitions-of-statistics-probability-and-key-terms | The question-first routine is an original teaching checklist. Distinguish descriptive, diagnostic, predictive and prescriptive labels as useful categories, not rigid universal taxonomy. |
| Data Quality Before Analysis | Check missing values, duplicates, row definitions, units, authorisation and privacy. | NIST Privacy Framework: https://www.nist.gov/privacy-framework; OpenStax statistics definitions: https://openstax.org/books/introductory-business-statistics/pages/1-1-definitions-of-statistics-probability-and-key-terms | The appropriate treatment of missing data depends on context. Do not automatically replace missing values with zero. |
| Descriptive Statistics and Segmentation | Interpret mean, median, rates and group comparisons. | OpenStax, *Introductory Business Statistics*, chapter 2 introduction: https://openstax.org/books/introductory-business-statistics/pages/2-introduction | Arithmetic check: values ₹100, ₹120, ₹130, ₹150 and ₹1,000 sum to ₹1,500; mean ₹300; median ₹130. Explain that neither summary is universally best. |
| KPIs, Funnels and Trends | Define metric numerator/denominator; calculate rates and avoid causal overclaiming. | OpenStax, *Introductory Business Statistics*, regression equation and assumptions: https://openstax.org/books/introductory-business-statistics/pages/13-4-the-regression-equation | 100/2,000 = 5%; 20/100 = 20%. These are fictional examples. The regression page is not a complete source for all KPI/funnel concepts; add exact causal inference/experiment sources if taught in depth. |
| SQL Thinking and Communicating Insights | Explain SELECT/FROM/WHERE/GROUP BY and communicate evidence with limitations. | SQLBolt: https://sqlbolt.com/; OpenStax statistics regression section: https://openstax.org/books/introductory-business-statistics/pages/13-4-the-regression-equation | SQLBolt is a practice resource, not scholarly research. Test the illustrative query against a sample schema before presenting it as executable in a particular database. |

## Knowledge check review
- First step question: answer 2.
- Missing-value question: answer False.
- Rate question: answer 2; 100/2,000 = 5%.
- Answer keys and arithmetic are internally consistent. The three-item quiz is not a validated assessment.

## Publication gate
Separate calculation correctness from interpretation quality. Keep simulated examples labelled, document dataset assumptions and privacy controls, and avoid treating correlation as causation. Keep the course labelled **source-mapped — review in progress**.

**Reviewer:** automated editorial/source-mapping pass; no independent statistics/data-protection expert review recorded.  
**Open work:** check all formulas and examples independently; add exact statistical inference/causal evidence references; test SQL against a defined schema; review privacy wording for target jurisdictions.
