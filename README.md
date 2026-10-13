# Commercial Revenue & Churn Decision Engine

A governed commercial decision product that analyzes customer acquisition, cohort retention, and revenue churn to advise an executive team on where growth is stalling and which intervention to fund next.

## Data

Online Retail II (UCI, CC BY 4.0): about 1M invoice lines from 2009 to 2011. It has no cost column, so state your margin assumption.

- [Online Retail II (UCI, CC BY 4.0)](https://archive.ics.uci.edu/dataset/502/online+retail+ii)

Built step by step on the [Stacc Data Analysis roadmap](https://app.getstacc.org/learn/da). Each module adds one verified
milestone to this repository; the commit history is the build log.

## Milestones

| # | Module | Adds to this repo | Verified |
|---|---|---|---|
| 01 | Exploratory Data Analysis | Decompose the business problem into a Metric Tree, formulate hypotheses, and profile missingness, cardinality, and outliers. | ☐ |
| 02 | Data Visualization | Create three statistical diagnostic charts (retention curve, LTV distribution, margin vs volume) with honest visual encoding. | ☐ |
| 03 | Dashboard Design | Architect desktop and mobile 3-tier dashboard layouts (Summary → Drill-Down → Action Table) adhering to the 5-second rule. | ☐ |
| 04 | Data Storytelling | Convert evidence into an executive briefing using the Minto Pyramid (SCQA) and an Amazon-style 1-pager decision memo. | ☐ |
| 05 | Governed BI Delivery | Implement the Power BI semantic model with Power Query ETL, Star Schema, Date table, explicit DAX, and dynamic RLS. | ☐ |
| 06 | AI-Assisted Analysis | Accelerate exploratory SQL/DAX with AI, sanitize PII, run independent verification assertions, and commit an AI log. | ☐ |
| 07 | End-to-End Decision Product | Release the entire decision system with green CI, data contracts, dashboard (.pbix / web embed), executive memo, and video walkthrough. | ☐ |

Tick a row when Stacc verifies the milestone. Replace this section's intro, but keep the table:
the first milestone checks that the plan is here.

<!--
Final demo question (answer it in the capstone walkthrough):
Where is revenue leaking across our customer cohorts, what operational intervention should the executive team fund next, and what evidence would invalidate that decision?

The capstone requires a "## Walkthrough" section in this README linking a
walkthrough of five minutes or less, and CI passing on the submitted commit.
-->
