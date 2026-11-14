# Prototype development and validation log

## Scope and provenance
- New AI-assisted demonstration added during final preparation on **November 14, 2026**; **not** represented as an earlier completed semester lab.
- Source: [cac-calculator.html](cac-calculator.html).
- Goal: distinguish ad-platform cost per conversion from CAC calculated using **user-supplied** new-customer counts, with strong input validation and explicit fictional-data labeling.
- Original team lab prompt/iteration history: not present in the repository. Add genuine earlier prompts and revisions only if available.

## Build prompt summary
Build a self-contained browser-based marketing CAC calculator with three channels and transparent sample values. Show aggregate spending, cost per platform-reported conversion, and cost per user-supplied new customer. Do not claim these inputs are real WOC CRM or order records. Validate nonnegative numbers, whole-person counts, impossible customer/conversion combinations, zero denominators, and reset behavior; do not store data or connect to third-party services.

## Executed functional verification — November 14, 2026

The **exact JavaScript embedded in this GitHub file** was fetched from the proposal branch and executed within an isolated JavaScript runtime against simulated DOM elements. These are scripted logic checks, **not yet a full end-to-end browser rendering test**.

| Scenario | Expected / observed result | Status |
|---|---|---|
| Starting inputs | Spend $4,700.00 | PASS |
| Starting reported conversions | Cost per conversion $16.21 | PASS |
| Starting new-customer inputs | Illustrative CAC $73.44 | PASS |
| Change Google Ads spend to $3,000 | Spend $5,300.00 | PASS |
| Recompute after spend change | Illustrative CAC $82.81 | PASS |
| New customers greater than conversions | Warning; calculations blocked | PASS |
| Negative spend | Warning; calculations blocked | PASS |
| Zero new customers on a channel | Channel CAC shows N/A | PASS |
| All denominators zero | Both rate metrics show N/A | PASS |
| Reset | Default illustrative CAC $73.44 restored | PASS |

**Data assumptions:** Google Ads: $2,400 / 110 conversions / 32 new customers; Instagram Ads: $1,800 / 95 / 20; Email: $500 / 85 / 12. All are hypothetical.

## Remaining manual QA and rubric evidence
- Open the **original HTML file** in Chrome/Edge; verify the full layout, labels and controls; capture a genuine screenshot.
- Repeat keyboard-only input, invalid input, mobile-width responsiveness and each failure case visually.
- Test the URL after the PR is merged and deployment is enabled; do not claim a published page before checking.
- Document actual student prompts and iterations; retain a screen recording or screenshots for final Slide 10.

## Important limitations
No connection to real WOC data; no deduplication of customer IDs; no proof of attribution; no business deployment. Displayed "CAC" is a demonstration of the formula **conditional on supplied counts being genuinely verified first-time customers**, not a real-world measurement.

## Chromium / Playwright browser verification — November 14, 2026

A separate **local browser test harness** was constructed with the **exact JavaScript logic** from `cac-calculator.html` (FNV-1a identifier `8b73a741`; 3,629 characters, verified identical). The harness used equivalent form IDs but simplified local CSS, so this verifies **browser execution and controls**, **not the complete original file's styling or remote deployment**.

Using Chromium through Playwright, **12 of 12 tests passed**: starting spend, cost per conversion, sample CAC, live recomputations after changing spend, impossible customer-count rejection, negative spend rejection, channel-level zero new customer handling, zero denominators, reset, no JavaScript page errors, and a mobile-width calculation check.

Screenshots were captured from the browser harness and a cropped view was placed into [the revised 11-slide Google Slides deck](https://docs.google.com/presentation/d/1JiU53bI1YgGB2jtGWRkKk16eN0A1mvKlJ7MuFDC2BTY/edit) on Slide 10. The slide must retain the illustrative-data disclosure. This does not prove WOC data integration or user-supplied new-customer counts are validated.

**Outstanding:** open and inspect the original HTML in a normal desktop/mobile browser, record genuine teammate prompt iterations if available, and verify publication after merge.
