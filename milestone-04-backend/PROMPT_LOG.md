# AI Assistance Log — WOC Marketing

**Date:** November 14, 2026

**My request (paraphrased):** I asked ChatGPT to verify our WOC-Marketing website and GitHub repository and identify what we needed to improve based on the final project grading rubric.

**What ChatGPT helped with:** It reviewed the repository and existing milestone artifacts, identified gaps against the rubric, improved the README and project documentation, created an example customer acquisition cost (CAC) calculator, tested its calculation logic, and helped prepare an updated executive presentation. I asked it to merge the reviewed improvements into the main GitHub branch.

**Important note:** The calculator uses fictional demonstration data, not WOC's actual customer data. This is a summary of our interaction rather than a verbatim copy of every prompt or the original semester-long development history.

## Follow-up AI coding improvement — November 14, 2026

**User's prompt:** "Can you help me improve my WOC Marketing customer acquisition cost calculator? I want users to enter advertising expenses, conversions, and new customers, then automatically calculate the results. Please explain what changes you're making to the code."

**AI-assisted edits:** Improved the existing calculator rather than rebuilding it. It already listened to `input` events and recalculated live. Added a per-channel cost-per-conversion column, a more explicit distinction between user-entered new customers and real verified CAC, totals for entered conversions/customers, improved money/count validation and accessible input/table labels. Corrected the chart so bar lengths represent the CAC metric being labeled instead of each channel's share of new customers.

**Iteration during testing:** An initial test showed the error message for fractional conversions was overwritten by an unrelated customer-count warning; the code was revised to prioritize malformed input. A separate test expectation was corrected because Instagram's illustrative CAC ($90) is higher than Google Ads' ($75), so Instagram should have the longest CAC bar.

**Observed results:** The exact JavaScript from this proposed GitHub branch passed **16 of 16 functional tests in an isolated V8 runtime with simulated DOM controls**, including live updates, sample totals, validation, zeros, comparison-bar widths and reset. This is not yet a complete visual/browser or deployed-site test.

**Example calculations (hypothetical):** $4,700 ad spend, 290 platform conversions and 64 user-entered new customers lead to $16.21 cost per conversion and $73.44 illustrative CAC. Entered customer counts must still be verified in a real system.

**Review before merge:** The code changes are proposed in a new pull request. They are a genuine November 14 refinement and should not be presented as earlier-semester work.
