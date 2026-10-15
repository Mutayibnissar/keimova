# Keimova QA Checklist

Last updated: 2026-10-15

## Scope and method
This checklist records static source checks and remaining manual checks. It is not a claim of successful browser, accessibility, or end-to-end testing. Run the pages in a real browser on desktop and mobile before public release.

## Static checks completed
- Inline JavaScript syntax checked with `new Function(...)` for the main catalogue, six course pages, shared course engine, dashboard, assessment centre, learning paths, project lab, study assistant, skills profile, and three business simulators.
- Duplicate HTML IDs checked on the pages included in the October 15 audit.
- Six course storage keys compared against the dashboard's expected keys.
- Generic Google Scholar discovery links removed from the main catalogue and the Business Analytics course; lesson-level sources should link to specific inspectable resources rather than a search-results page.
- Storage failure and malformed-data handling improved in the course engine, dashboard, assessment centre, learning paths, project lab, study assistant, and main catalogue.
- Pricing & Cash Flow Lab now rejects blank/invalid values and clears stale results before export.
- Marketing Budget Simulator rejects blank/invalid inputs and clears stale displayed results.
- Business Break-Even Calculator rejects blank inputs and clears stale displayed results.

## Manual browser test plan
- [ ] Main catalogue: tab/category/level filters, search, sorting, modal open/close, keyboard Escape, mobile menu, save item, start item, and My Learning with empty and malformed stored values.
- [ ] Course pages: complete a lesson, navigate between lessons, answer quiz correctly/incorrectly, refresh, export notes/progress, reset, and confirm dashboard reflects the same state.
- [ ] Course engine: test with browser storage enabled, disabled, and quota/error simulation where possible; confirm status feedback and no false success message.
- [ ] Dashboard: empty state, partially completed courses, assessment history, project history, JSON export, and reset confirmation.
- [ ] Assessment centre: each quiz mode, answer feedback, retry, exit, saved history, malformed history, and storage unavailable.
- [ ] Learning paths: generate recommendations, save, reload, clear, and storage unavailable.
- [ ] Project Lab: open all briefs, validate required fields, review, save, load, delete, export, clear history, and storage unavailable.
- [ ] Study Assistant: generate a guide, endpoint validation, saved endpoint reload/removal, and behaviour when local storage or AI backend is unavailable.
- [ ] Skills Profile: course counts, assessment/project rendering, export, malformed stored JSON, and storage unavailable.
- [ ] Simulators: valid inputs, blank fields, boundary values, invalid values, recalculation after an error, and no stale result/export.
- [ ] Accessibility: keyboard-only use, focus visibility, labels, live-region announcements, contrast, reduced-motion preference, zoom to 200%, and screen-reader spot checks.
- [ ] Responsive: test at narrow mobile widths, tablet, and desktop; verify no horizontal overflow or clipped controls.
- [ ] Deployment: check GitHub Pages build, all internal links, browser console/network errors, and direct page refresh on nested paths.

## Content and evidence release gate
- [ ] Verify each lesson objective and material claim against the exact cited source section/page.
- [ ] Record source version/date, review date, evidence limitations, and license/reuse status in the course audit.
- [ ] Inspect primary research where a lesson makes empirical claims; do not treat Google Scholar search results as evidence.
- [ ] Review copyright and commercial reuse permissions before reusing/adapting third-party teaching materials.
- [ ] Obtain independent subject-matter review for business, marketing, HR/employment-law, finance, analytics/privacy, and AI-governance content as appropriate.
- [ ] Keep curriculum status as **source-mapped — review in progress** until the relevant gates are complete.

## Release rule
Do not advertise courses as “verified,” “research-backed,” or “peer-reviewed” solely because sources are listed. Do not claim browser, end-to-end, accessibility, or production deployment tests passed unless those checks were actually performed and recorded.
