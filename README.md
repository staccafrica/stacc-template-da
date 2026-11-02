# Revenue and churn analysis

An analysis of a real online retailer: where revenue is lost across customer cohorts, and which fix the leadership team should fund next.

## Data

Online Retail II (UCI, CC BY 4.0): about 1M invoice lines from 2009 to 2011. It has no cost column, so state your margin assumption.

- [Online Retail II (UCI, CC BY 4.0)](https://archive.ics.uci.edu/dataset/502/online+retail+ii)

Built step by step on the [Stacc Data Analysis roadmap](https://app.getstacc.org/learn/da). Each module adds one verified
milestone to this repository; the commit history is the build log.

## Milestones

| # | Module | Adds to this repo | Verified |
|---|---|---|---|
| 01 | Exploratory Data Analysis | Write the decision and metric tree, then profile the data for missing values, duplicates and outliers. | ☐ |
| 02 | Data Visualization | Make three honest charts: cohort retention, customer value, and margin against volume. | ☐ |
| 03 | Statistics for Analysts | Read an A/B test, compare groups with chi-square or ANOVA and find what drives revenue with regression, each with its limits. | ☐ |
| 04 | Dashboard Design | Design a desktop and phone dashboard: summary, drill-down and action table. | ☐ |
| 05 | Data Storytelling | Write a one-page memo and a five-slide deck that lead with the recommendation and its cost. | ☐ |
| 06 | Power BI | Build the Power BI model with a star schema, date table, DAX measures and row-level security, saved as a Power BI Project. | ☐ |
| 07 | AI-Assisted Analysis | Use AI to draft SQL or DAX, then prove each result against your own numbers before you keep it. | ☐ |
| 08 | Analysis Capstone | Release the analysis with green CI and a design doc, publish the report to a live page that refreshes itself, and add the memo and a walkthrough video. | ☐ |

## Acceptance evidence

Use the guided fixture and the independent variation in each module. Fix failures, then rerun every earlier test on the same candidate commit.
The filenames below are the submission contract, not supplied solutions. Implement the tests and artifacts yourself; do not commit generated caches or personal data.

### Exploratory Data Analysis

- `README.md`
- `brief.md`
- `notebooks/01_eda_profiling.ipynb`
- `data_quality_register.md`
- `tests/test_revenue_reconciliation.py`

### Data Visualization

- `src/charts.py`
- `visual_qa_audit.md`
- `tests/test_cohorts.py`
- `reports/chart_evidence.md`

### Statistics for Analysts

- `src/stats_tests.py`
- `reports/stats_tests.md`
- `tests/test_stats.py`

### Dashboard Design

- `specs/dashboard_architecture.md`
- `reports/usability_observations.md`

### Data Storytelling

- `briefing/executive_memo.md`
- `briefing/presentation_deck.pdf`
- `briefing/sensitivity.csv`

### Power BI

- `bi/metric_dictionary.md`
- `bi/refresh_runbook.md`
- `bi/project/Revenue.pbip`
- `bi/project/Revenue.Report/definition.pbir`
- `bi/project/Revenue.SemanticModel/definition.pbism`
- `bi/acceptance_results.csv`
- `reports/dashboard_evidence.md`
- `tests/test_bi_reconciliation.py`
- `bi/project/Revenue.Report/definition/report.json`
- `bi/project/Revenue.SemanticModel/definition/model.tmdl`

### AI-Assisted Analysis

- `AI_USE.md`
- `ai/prompt_templates.md`
- `tests/test_ai_reconciliation.py`

### Analysis Capstone

- `README.md`
- `briefing/executive_memo.md`
- `reports/uncertainty_register.md`
- `reports/qa_checklist.md`
- `AI_USE.md`
- `bi/project/Revenue.pbip`
- `bi/project/Revenue.Report/definition.pbir`
- `bi/project/Revenue.SemanticModel/definition.pbism`
- `bi/acceptance_results.csv`
- `reports/dashboard_evidence.md`
- `tests/test_release_acceptance.py`
- `bi/project/Revenue.Report/definition/report.json`
- `bi/project/Revenue.SemanticModel/definition/model.tmdl`
- `docs/design.md`
- `.github/workflows/publish.yml`

Keep the assessment job named `test` in GitHub Actions. It must run the actual acceptance tests; a green empty workflow does not establish correctness.
For non-Python artifacts, add the appropriate validation/integration commands to CI and retain their outputs.
Stacc's automatic checks establish artifact structure and CI status. Use the module criteria to assess numerical correctness, design quality and independent understanding.

Tick a row when Stacc verifies the milestone. Replace this section's intro, but keep the table:
the first milestone checks that the plan is here.

<!--
Final demo question (answer it in the capstone walkthrough):
Where is revenue being lost across customer cohorts, what should the team fund next, and what evidence would change your mind?

The capstone requires a "## Walkthrough" section in this README linking a
walkthrough of five minutes or less, and CI passing on the submitted commit.
-->
