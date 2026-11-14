# WOC Marketing — IS 3060 Consulting Challenge

**Client:** Wasatch Outfitters Collective (WOC), a fictional consulting case  
**Track:** G — Marketing  
**University:** University of Utah  
**Team:** Shawn Parkin · Sean Siracusa · Kallie Northrop · Ella Todd · Evelyn Teoyotl Rojas

**Project website:** [WOC Marketing homepage](https://shawncparkin.github.io/WOC-Marketing/) *(GitHub Pages availability must be confirmed)*  
**Prototype:** [Interactive CAC calculator](milestone-04-backend/cac-calculator.html)  
**Presentation:** [Editable 11-slide executive deck](https://docs.google.com/presentation/d/1JiU53bI1YgGB2jtGWRkKk16eN0A1mvKlJ7MuFDC2BTY/edit) *(Google Slides sharing/access must be confirmed)*

## Business problem and recommendation

WOC's marketing reports come from separate advertising and email platforms, limiting its ability to compare spending and understand how many **first-time customers** each channel brings in. Platform-reported conversions are not necessarily unique new customers.

**Recommendation:** Pilot a practical marketing measurement process connecting channel spending, verified customer identity, and sales records. Apply consistent definitions and quality checks, then use a shared dashboard to support budgeting decisions. Start with a small pilot rather than replacing every platform at once.

**Metric definitions:**
- **Cost per reported conversion:** Advertising spend ÷ platform-reported conversions.
- **New-customer acquisition cost (CAC):** Attributable acquisition spend ÷ verified first-time customers over the same period.
- The two metrics **are not interchangeable**. Real CAC also requires deduplication, agreed attribution rules, and reliable source data.

## Project artifacts and owners

The links below point to actual repository files or folders. **Uploaded** means a file is present in GitHub, not that the entire milestone has been approved or graded.

| Milestone | Artifacts and current status | Owner and presentation use |
|---|---|---|
| [1 · Tableau](milestone-01-tableau/) | **Uploaded:** [dashboard image](milestone-01-tableau/WOC_Marketing_Dashboard.png), [Tableau workbook](milestone-01-tableau/WOC_Marketing_Dashboard_Final.twbx), [written analysis](milestone-01-tableau/WOC_Tableau_Performance_Analysis_Revised_Sean.docx) | **Sean Siracusa** — marketing analysis, Slide 4 |
| [2 · SQL](milestone-02-sql/) | **Uploaded:** [SQL analysis](milestone-02-sql/WOC_Track_G_SQL_Final_Organized_Sean.docx), [relationship diagram](milestone-02-sql/sql_foreign_key_relationships.png), [SQL screenshot document](milestone-02-sql/sql%20screenshot.docx) | **Sean Siracusa** — data relationships and future-state logic, Slides 5–6 |
| [3 · Wix and cloud](milestone-03-wix-cloud/) | **Evidence pending:** folder exists, but Wix screens and a documented platform comparison are not uploaded | **Kallie Northrop** — solution design and technology selection, Slide 7 |
| [4 · AI-assisted prototype](milestone-04-backend/) | **Prototype and documentation uploaded:** [CAC calculator](milestone-04-backend/cac-calculator.html), [AI prompt and iteration log](milestone-04-backend/PROMPT_LOG.md), [test and demonstration guide](milestone-04-backend/README.md). Previous testing includes **12/12 browser-harness checks** and **16/16 isolated JavaScript/DOM checks**; Shawn reports **5/5 live Chrome manual tests passed**, with [a recording](https://drive.google.com/file/d/1PehbrF5-JSJDL8b5y9qeaOM6VpJAOQhC/view) and [screenshot](https://drive.google.com/file/d/1fOs3_Kf23xJ7hUCvGlJ5MmnERNEv7E8x/view) available; the live Chrome demonstration is included on Slide 10 and both media links allow anyone with the link to view; Shawn also confirmed that the website and calculator worked on his phone | **Shawn Parkin** — prototype and GitHub coordination, Slide 10 |
| [5 · Cybersecurity](milestone-05-cybersecurity/) | **Partial:** [risk-register template](milestone-05-cybersecurity/RISK_REGISTER_TEMPLATE.md) uploaded; final assessed likelihood, impact, owner, and controls are **not yet uploaded** | **Ella Todd** — risk and governance, Slide 9 |
| [6 · Implementation](milestone-06-implementation/) | **Partial:** [marketing information design document](milestone-06-implementation/WOC_Marketing_Information_Design_System.docx) uploaded; phased plan, owners, adoption steps, and metrics require confirmation | **Ella Todd**, with **Evelyn Teoyotl Rojas** coordinating presentation integration — Slide 11 |
| [Executive presentation](final-presentation/) | **Editable draft available:** [11-slide Google Slides deck](https://docs.google.com/presentation/d/1JiU53bI1YgGB2jtGWRkKk16eN0A1mvKlJ7MuFDC2BTY/edit) and [rubric evidence map](final-presentation/RUBRIC_EVIDENCE_MAP.md). A final PowerPoint file **has not been committed** to the repo | **Evelyn Teoyotl Rojas** coordinates final integration; **all five teammates** review and present |

**Shawn Parkin and Sean Siracusa are different team members.** Shawn leads the prototype/GitHub effort; Sean leads Tableau/SQL analysis.

## Evidence-backed findings

Sean's [Tableau performance analysis](milestone-01-tableau/WOC_Tableau_Performance_Analysis_Revised_Sean.docx) reports cost per conversion of **$2.91** for Email Newsletter, **$12.87** for Instagram Ads, **$40.55** for Google Search, and **$41.53** for Local Radio. Email has the lowest reported conversion cost in that analysis. These values are **not independently verified new-customer CAC**.

The [CAC calculator](milestone-04-backend/cac-calculator.html) is an AI-assisted educational prototype. It uses **fictional sample inputs**, updates calculations automatically, and checks invalid values. It neither connects to a real CRM nor verifies customer identities or campaign attribution. Read the [development log](milestone-04-backend/PROMPT_LOG.md) for genuine prompts, coding iterations, tests, and linked screenshots.

## Outstanding work before final submission

- [ ] **Kallie:** Upload actual Wix/cloud screenshots and an evaluated platform recommendation with cost, fit, scalability, and risk considerations.
- [ ] **Ella:** Upload a completed WOC-specific risk register with **at least three rated risks** (likelihood, impact, control) and confirm the implementation plan.
- [ ] **Team — Slide 8:** Add an actual AI/CRM interaction test, its observed result, a failure/escalation case, and human oversight.
- [ ] **Team — Slides 5–6:** Confirm the real current-state process map, bottlenecks, future-state joins, and information flows.
- [x] **Shawn:** **Desktop Chrome tests passed (5/5 manual checks), and phone layout/functionality confirmed by Shawn.** The [recording](https://drive.google.com/file/d/1PehbrF5-JSJDL8b5y9qeaOM6VpJAOQhC/view) and [screenshot](https://drive.google.com/file/d/1fOs3_Kf23xJ7hUCvGlJ5MmnERNEv7E8x/view) are now linked from Milestone 4. Slide 10 now includes the real screenshot and embedded video, and both test media files are shared for viewing. Mobile validation is complete based on Shawn's report; AI screenshots remain externally linked rather than committed image binaries.
- [ ] **Evelyn and team:** Replace draft slide claims with approved evidence, confirm the phased 30-day/60–90-day/6–12-month roadmap and adoption metrics, upload the **final** PowerPoint into `final-presentation/`, and rehearse.

## Repository and integrity notes

The detailed rubric scores the repository **15 points** and presentation **85 points**; a contradictory 20/80 sentence also appears in its closing text. Confirm any ambiguity with the instructor. See the [rubric evidence map](final-presentation/RUBRIC_EVIDENCE_MAP.md).

Preserve actual commit dates and attribute work correctly. Do not invent missing lab evidence, earlier prompts, real business data, risk scores, or results that have not been tested.