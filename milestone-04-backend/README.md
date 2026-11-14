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
- **Live Chrome test (November 14, 2026):** Shawn reports all **five manual checks passed** on the published calculator and supplied a genuine ~28-second screen recording and screenshot. The inspected video shows the default values, calculations changing as inputs are edited, and an invalid-entry warning. This complements—but is separate from—the earlier automated tests. The video and screenshot are shared as viewable links. **Mobile check (November 14, 2026):** Shawn confirmed that the website and calculator worked correctly on his phone. This is student-reported manual testing, not an independently reproduced device test.
- The [prompt log](PROMPT_LOG.md) includes genuine conversation prompts, revisions, and **links to two screenshots hosted in Google Drive**. The AI conversation images are linked from Google Drive rather than embedded in this GitHub repository.

## Suggested demonstration

1. Open [the actual calculator](cac-calculator.html), explain the fictional-data warning, and identify the two different metrics.
2. Change Google Ads spend from $2,400 to $3,000; the total should move to $5,300 and illustrative CAC to $82.81.
3. Enter a negative spend or more new customers than reported conversions; show the validation message.
4. Enter zero new customers for a channel; show N/A for that channel's CAC.
5. Reset the example and explain what verified records would be required for real CAC.

**Rubric integrity:** The new calculator was created during November 2026 final-project preparation and is not evidence of an earlier completed semester lab. The log records the interactions that actually occurred.

## Actual browser evidence

- [Shawn's live Chrome calculator recording (~28 seconds)](https://drive.google.com/file/d/1PehbrF5-JSJDL8b5y9qeaOM6VpJAOQhC/view)
- [Screenshot of starting calculator totals](https://drive.google.com/file/d/1fOs3_Kf23xJ7hUCvGlJ5MmnERNEv7E8x/view)

Shawn reported **5 of 5 manual tests passed**. These files are currently linked from Google Drive (not committed as binary files to GitHub). Both files are shared as viewable links and appear on the updated Slide 10; keep a local copy available for presentation playback.
