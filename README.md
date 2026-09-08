# NovaTech Revenue Intelligence Dashboard

A three-sheet Amazon Quick (QuickSight) dashboard — Marketing Funnel, Sales Pipeline, and
Customer Health — built on NovaTech's CRM, marketing and support data, plus the natural-language
(Topic/Q) layer configured on top of it.

## Contents

- **docs/** — the written deliverables
  - `NovaTech_05_Report_Sarah_Chen.md` / `.pdf` — the final report to the VP of Revenue: what was
    built, the two data-honesty caveats, what the Topic changed, the five findings and
    recommendations, and where the AI agreed or disagreed with the verified numbers.
  - `NovaTech_01_Verification_Log.md` — the log of figures verified directly against the source
    CSVs before they were trusted in any chart or answer.
  - `NovaTech_04_Topic_and_Q_Log.md` — the Topic build spec, the three-question before/after
    baseline (B1–B3), and the five-question post-Topic exploration log (Q1–Q5).
  - `NovaTech_00_Verified_Figures.md` — the reference set of verified numbers the dashboard and
    report are checked against.
  - `NovaTech_02_Data_Prep_Spec.md` — the join logic and data-prep steps (joins, calculated
    fields, data type corrections).
  - `NovaTech_03_Dashboard_Build_Plan.md` — the sheet-by-sheet visual build plan.
  - `NovaTech_README_Rubric_Map.md` — how the deliverables map to the project rubric.
- **data/** — the three source CSVs (CRM deals, marketing campaigns, support tickets).
- **reference/** — the original project brief and data dictionary supplied with the exercise.
- **evidence/** — screenshots captured live during the build: the join diagram and join
  configuration, the calculated-field formulas, the data-type-correction step, the Topic
  configuration, the before/after Quick Chat answers (B1–B3, P1–P3), the Q Exploration Log
  questions and answers, the dashboard sheets, and the annotated dashboard. Filenames are capture
  timestamps in chronological order; the narrative in `NovaTech_04_Topic_and_Q_Log.md` and
  `NovaTech_01_Verification_Log.md` describes what each stage of screenshots shows.

## Key finding

The Topic's semantic layer reliably fixed vocabulary ambiguity (e.g. "conversion rate" meaning
closed-won rate, not response rate) but did not reliably override the tool's default aggregation
behaviour on a join-shaped question, even with an explicit written rule. Full detail is in the
report's "What the Topic changed" section.
