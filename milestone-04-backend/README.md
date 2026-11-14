# Milestone 4 — AI-Assisted CAC Calculator Prototype

**Owner:** Shawn Parkin — prototype and GitHub coordination  
**Code:** [cac-calculator.html](cac-calculator.html)  
**AI development and iteration record:** [PROMPT_LOG.md](PROMPT_LOG.md)  
**Project homepage:** [WOC Marketing website](../index.html)

## What the prototype actually does

This self-contained HTML, CSS, and JavaScript example lets users edit three channels' **advertising spend**, **platform-reported conversion count**, and **user-entered new-customer count**. It recalculates totals, channel-level cost per conversion, and **illustrative** channel CAC as values change. It checks invalid and impossible inputs and displays N/A instead of dividing by zero. The comparison bars represent the magnitude of channel CAC.

**Example data are fictional:** $4,700 total spend, 290 platform conversions, and 64 entered new customers, producing **$16.21 per conversion** and **$73.44 illustrative CAC**.

## Important limitation

The tool does **not** import WOC's actual campaigns, CRM, or transaction data. It does not verify whether a customer is genuinely new, deduplicate across platforms, or establish real attribution. **Cost per conversion is not verified CAC.** The website is a student proof of concept, not a production analytics system.

## AI assistance and tests

- ChatGPT helped review the project against the rubric and improve the calculator's HTML, CSS, and JavaScript.
- An earlier version passed **12/12 Chromium checks using a local browser test harness with the same core JavaScript**.
- The improved JavaScript passed **16/16 functional checks in an isolated V8 runtime with simulated DOM inputs**.
- **Still needed:** test the revised original HTML visually in a normal desktop/mobile browser, confirm the GitHub Pages URL actually serves it, and capture a demonstration. Do not portray the prior tests as fully validating the deployed site.
- The [prompt log](PROMPT_LOG.md) includes genuine conversation prompts, revisions, and **links to two screenshots hosted in Google Drive**. The images are not embedded in this GitHub repository; check instructor access.

## Suggested demonstration

1. Open [the actual calculator](cac-calculator.html), explain the fictional-data warning, and identify the two different metrics.
2. Change Google Ads spend from $2,400 to $3,000; the total should move to $5,300 and illustrative CAC to $82.81.
3. Enter a negative spend or more new customers than reported conversions; show the validation message.
4. Enter zero new customers for a channel; show N/A for that channel's CAC.
5. Reset the example and explain what verified records would be required for real CAC.

**Rubric integrity:** The new calculator was created during November 2026 final-project preparation and is not evidence of an earlier completed semester lab. The log records the interactions that actually occurred.

[Back to project README](../README.md).