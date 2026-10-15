# Keimova — Learn. Apply. Evolve.

Keimova is a responsive learning-hub prototype for practical business, career and technology learning. Its information architecture is inspired by modern resource hubs, with category shortcuts, searchable catalogues, filters and learning-item previews. Keimova uses its own name, visual identity and original sample copy.

## Current prototype
- Five catalogues: Courses, Roadmaps, Masterclasses, Resources and Simulators
- Two dedicated interactive courses: Business Administration Essentials and Marketing Strategy & Growth, each with five lessons, completion tracking, quiz feedback and further-reading links
- First interactive course: `courses/business-administration-essentials.html` with five lessons, completion tracking, knowledge-check feedback and source links
- Search, subject filters, level filters and alphabetical sorting
- Learning-item detail modals with learning objectives and topic-specific Google Scholar/trusted reference links
- Evidence-source hierarchy and publishing/review checklist in `SOURCES.md`
- Save-for-later and started-learning lists using browser `localStorage`
- Responsive desktop/mobile navigation and reduced-motion support
- Sample content across Business Administration, Marketing, HR, Finance, Analytics, AI & Technology, and Career Skills

## Evidence-based curriculum
- `SOURCES.md` documents source quality rules, citation expectations and review workflow.
- `curriculum/STARTER_CURRICULUM.md` maps five starter courses to learning outcomes, lesson sequences, assessments and initial authoritative references.
- Item detail modals provide topic-specific Google Scholar searches and selected official/professional references. These links are discovery aids; the sample catalogue is not yet fully fact-checked or peer-reviewed.

## Run locally
Open `index.html` in a modern browser. No build step or package installation is required.

## Publish with GitHub Pages
1. Open the repository's **Settings → Pages**.
2. Under **Build and deployment**, choose **Deploy from a branch**.
3. Select the `main` branch and `/(root)`, then save.
4. Wait for deployment to finish and open the URL shown in Settings → Pages.

## Prototype limitations
This is a front-end prototype. Progress and saved items are stored only in the current browser; they do not sync between devices. Sample lessons, workshops and simulators are illustrative, not a complete course delivery system. The source links are research-discovery aids; they do not mean the sample course content has already been fully fact-checked or peer-reviewed. Authentication, database persistence, an AI tutor, complete course content and production browser testing still need to be implemented.

## Reference and originality
Reference: https://resources.criodo.com/. Keimova adapts broad resource-hub interaction patterns rather than using Crio branding or claiming affiliation with Crio.Do.


## Interactive learning tools

- **My Learning Dashboard:** `dashboard/index.html` — summarizes locally stored course completion, quiz scores, saved items and started catalogue items; supports JSON progress export and course-progress reset.
- **Marketing Budget Simulator:** `tools/marketing-budget-simulator.html` — models clicks, conversions, revenue, gross profit, modeled net, ROAS, break-even conversions and alternative conversion-rate scenarios; supports CSV export.
- **Interactive courses:** `courses/business-administration-essentials.html` and `courses/marketing-strategy-growth.html`.

All progress remains in browser local storage. There is no account system or cloud synchronization. Simulator outputs are assumption-based estimates, not forecasts. Full browser/device testing and live Pages deployment still need verification.
