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

## Screenshot-backed ChatGPT prompts — November 14, 2026

These are actual conversations documented by the two screenshots I provided to ChatGPT. Original screenshot images are preserved as linked Google Drive evidence; the images are **not stored as GitHub repository binaries**. They should not be presented as interactions from earlier in the semester.

### Evidence A — Website code and rubric review
**Screenshot evidence:** [View original code review screenshot](https://drive.google.com/file/d/1RyxvnJ9P-gptRFJ4RdDegJVMz28SOfQ6/view?usp=drivesdk) (uploaded as `chat doing it's thing.PNG`)

**My exact prompt:**
> Can you review the HTML, CSS, and JavaScript for my WOC Marketing website and identify any errors or improvements? I want to make sure everything works correctly and meets my KPMG final project rubric.

**What ChatGPT identified:** The general homepage still had placeholder teammates and outdated milestone status information; it lacked a direct link to the CAC calculator; mobile navigation was hidden; the page should emphasize our Marketing track; and the calculator's comparison-bar widths originally measured customer share even though the labels showed CAC. ChatGPT explained how these issues relate to the rubric's functioning-prototype and professional-communication criteria.

**What I learned:** Reviewing the source code against specific grading requirements helped prioritize corrections to the page and the demo.

### Evidence B — Calculator coding improvement
**Screenshot evidence:** [View original calculator improvement screenshot](https://drive.google.com/file/d/1EUjO3Fr-0s4wIFL_l4w3SCaLZbqoy7lJ/view?usp=drivesdk) (uploaded as `chat doing its thing again.PNG`)

**My exact prompt:**
> Can you help me improve my WOC Marketing customer acquisition cost calculator? I want users to enter advertising expenses, conversions, and new customers, then automatically calculate the results. Please explain what changes you're making to the code.

**Changes made with AI assistance:** ChatGPT improved the existing HTML, CSS and JavaScript rather than recreating the calculator. The changes added per-channel cost per conversion alongside illustrative CAC; clearer automatically updating totals; input validation for negative, fractional and invalid values; more accurate comparison-bar lengths; and clearer explanations that the figures use fictional data.

**Coding iteration and verification:** One test exposed an error-message priority issue when a fractional conversion count was entered, which led to a code correction. The updated JavaScript then passed **16 of 16 functional tests with simulated DOM controls**. The tests are evidence of calculation logic, not complete visual testing of the public site.

**Fictional demonstration totals:** $4,700 in advertising spend, $16.21 cost per conversion, and $73.44 illustrative CAC. This is not verified real WOC CAC.

**Code change:** [Pull Request #3](https://github.com/shawncparkin/WOC-Marketing/pull/3).

### Screenshot upload status
Both original screenshot files are linked above from the project's Google Drive evidence copies. They are **not embedded in the GitHub repository**, and access for instructors depends on Google Drive sharing permissions. For a completely self-contained GitHub submission, upload both PNGs to `milestone-04-backend/evidence/` and use relative Markdown links instead.
