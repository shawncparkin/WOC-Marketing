# WOC Marketing — IS 3060 Consulting Challenge

**Client:** Wasatch Outfitters Collective (WOC; fictional class case)  
**Track:** G — Marketing  
**University:** University of Utah  
**Team:** Ella Todd, Shawn Parkin, Kallie Northrop, Sean Siracusa, Evelyn Rojas

## Executive recommendation

WOC should pilot a **lightweight, governed marketing measurement workflow** that connects channel spending to deduplicated customer and sales records. This will enable more trustworthy channel comparisons and, where records are sufficiently complete, calculation of **new-customer acquisition cost (CAC)**.

WOC's marketing data is fragmented among advertising and email platforms. Platform-reported conversions cannot automatically be equated with first-time customers. The proposal therefore prioritizes consistent identifiers, verified new-customer definitions, transparent data-quality checks, an executive dashboard, and phased implementation rather than an expensive company-wide replacement.

**Metric definitions**
- **Cost per reported conversion:** channel spending / reported platform conversions.
- **New-customer CAC:** attributable acquisition spending / verified first-time customers acquired over a consistent period.
- These figures are **not interchangeable**. Zero denominators, duplicates, missing source IDs, attribution assumptions, and existing-customer activity must be flagged.

## Project artifacts

| Folder | Evidence presently in the repository | Owner / rubric use |
|---|---|---|
| [Milestone 1: Tableau](milestone-01-tableau/) | [Dashboard PNG](milestone-01-tableau/WOC_Marketing_Dashboard.png), [Tableau workbook](milestone-01-tableau/WOC_Marketing_Dashboard_Final.twbx), [written analysis](milestone-01-tableau/WOC_Tableau_Performance_Analysis_Revised_Sean.docx) | Sean — dashboard evidence, Slide 4 |
| [Milestone 2: SQL](milestone-02-sql/) | [SQL analysis](milestone-02-sql/WOC_Track_G_SQL_Final_Organized_Sean.docx), [foreign-key diagram](milestone-02-sql/sql_foreign_key_relationships.png), [SQL screenshot document](milestone-02-sql/sql%20screenshot.docx) | Sean — data relationships and solution logic |
| [Milestone 3: Wix + cloud](milestone-03-wix-cloud/) | Folder established; **Wix screenshots and platform comparison not yet in repository** | Kallie — interface concept and platform selection |
| [Milestone 4: Prototype](milestone-04-backend/) | [New sample-only CAC calculator](milestone-04-backend/cac-calculator.html) and [development record](milestone-04-backend/PROMPT_LOG.md); **does not replace original course lab evidence** | Shawn — working demonstration; needs real testing and recorded iteration history |
| [Milestone 5: Cybersecurity](milestone-05-cybersecurity/) | Folder established; [risk-register working template](milestone-05-cybersecurity/RISK_REGISTER_TEMPLATE.md). **Final team ratings still required** | Ella — risk register and practical controls |
| [Milestone 6: Implementation](milestone-06-implementation/) | [Marketing information design document](milestone-06-implementation/WOC_Marketing_Information_Design_System.docx); phased plan still to validate | Ella / Evelyn — owner-based rollout, governance, success metrics |
| [Final presentation](final-presentation/) | [Slide evidence and readiness audit](final-presentation/RUBRIC_EVIDENCE_MAP.md). **Final slide deck not yet uploaded** | Whole team — executive recommendation |

## Suggested solution flow

1. Collect advertising spend, platform-reported activity, customer identity and sales outcomes.
2. Normalize channels, time periods, campaign identifiers and customer definitions.
3. Join data carefully, deduplicate and flag missing or conflicting records.
4. Publish dashboard comparisons with explicit definitions and uncertainty indicators.
5. Pilot automation only for **flagging anomalies or drafting recommendations**; require human validation before changing official metrics or spending.
6. Expand to additional locations and channels after an initial pilot passes data-quality and user-adoption checks.

## Proof of concept

The [sample CAC calculator](milestone-04-backend/cac-calculator.html) is an **educational, AI-assisted demonstration added during final-project preparation**. Open the HTML file in a browser, or view it at [the project Pages path](https://shawncparkin.github.io/WOC-Marketing/milestone-04-backend/cac-calculator.html) **if GitHub Pages is enabled and published**.

It works with expressly *fictional*, editable marketing figures; it does not connect to WOC datasets or validate real new-customer identities. See [prototype instructions](milestone-04-backend/README.md) and [development notes](milestone-04-backend/PROMPT_LOG.md).

The existing root [`index.html`](index.html) is a **general course-project website**, not the CAC calculator or a deployed data pipeline.

## Final evaluation

Use [the rubric-to-evidence map](final-presentation/RUBRIC_EVIDENCE_MAP.md) before submitting. It distinguishes **verified files**, **proposed solutions**, and **missing evidence**. Do not present illustrative prototype numbers as dashboard findings or claim that controls or outcomes have been validated when they have not.

**Version-control integrity:** retain real commit dates and meaningful messages; do not reconstruct a fictional semester-long history. Future source artifacts should be committed as completed.
