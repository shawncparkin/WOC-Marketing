# Milestone 4 — Sample CAC Calculator (new final-prep proof of concept)

**Open:** [cac-calculator.html](cac-calculator.html) in a modern browser. No installation, API keys or network access is required. If GitHub Pages is enabled, it may also be opened via the matching Pages path; validate that link before presenting.

## Purpose and actual capabilities
The static HTML page demonstrates the **calculation layer** of a proposed WOC marketing reporting workflow. Enter ad spend, platform conversions and user-supplied counts of verified new customers for three channels. It displays channel-level and portfolio-level cost-per-conversion and CAC, with warnings for impossible or missing inputs and safe handling of division by zero.

The built-in values are **hypothetical** (total spend $4,700; 290 conversions; 64 new customers). They produce cost per conversion **$16.21** and CAC **$73.44** when rounded to cents.

**Limitations:** It does not ingest actual Tableau/CRM/ad-platform data, validate customer identity, attribute sales, preserve state, or perform AI inference. It is not evidence that WOC's real CAC has been determined. The root [index.html](../index.html) is a separate general WOC landing page.

## Demonstration checklist
1. Open the calculator in a browser and show the sample-data disclosure.
2. Explain cost per reported conversion versus spend per verified new customer.
3. Change Google Ads spend from 2,400 to 3,000 and verify the results update.
4. Set one channel's new-customer count to 0 and show its channel CAC becomes N/A.
5. Enter more new customers than conversions and show the validation warning.
6. Reset the sample inputs. Record a real screenshot and your observed results for final Slide 10.

**Functional test update (Nov 14, 2026):** The exact JavaScript was checked in Chromium via a styled local test harness; 12/12 browser checks passed. See [PROMPT_LOG.md](PROMPT_LOG.md). Deployment and direct visual QA of this original HTML file are still pending. The revised [executive presentation](https://docs.google.com/presentation/d/1JiU53bI1YgGB2jtGWRkKk16eN0A1mvKlJ7MuFDC2BTY/edit) contains a screenshot of that browser harness and explanatory notes.\n\n**Rubric integrity:** This is a new AI-assisted prototype created during final preparation. It must not be represented as a completed earlier lab. Add actual prompts, iterations, test dates and observed outcomes in [PROMPT_LOG.md](PROMPT_LOG.md) as they occur.
