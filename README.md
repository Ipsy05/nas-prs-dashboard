# India Grade 3 — NAS/PRS Learning Outcomes Dashboard

An interactive dashboard analyzing India's Grade 3 student learning outcomes across three national assessment rounds — **NAS 2017**, **NAS 2021**, and **PRS 2024** — at the national and state level.

**[View the live dashboard →](#)** *(link will work once GitHub Pages is enabled — see setup below)*

## What this is

NAS (National Achievement Survey) and PRS (PARAKH Rashtriya Sarvekshan) are India's largest system-level assessments of student learning outcomes, conducted by NCERT/PARAKH. They are not student exams — no child receives an individual score. Results are reported at the district, state, and national level, and are used to guide programs like NIPUN Bharat, teacher training, and budget allocation. Grade 3 is the only grade tested in a comparable format across all three rounds (2017, 2021, 2024), which makes it the sole basis for a genuine longitudinal comparison.

This project pulls together publicly available NAS/PRS data across the three rounds into a single interactive dashboard, and draws out the key patterns, equity gaps, and policy-relevant findings the raw numbers contain.

## Key findings

- **The recovery paradox**: the national average score in 2024 (62.0%) is still below the 2017 baseline (65.7%) — yet *more* children now clear the proficiency bar than in 2017. Top performers recovered fast after COVID; the bottom 35–40% did not, and the average conceals this.
- **A 15-year equity gap that hasn't closed**: SC/ST students score ~8 percentage points below the General category, in both 2017 and 2024 — the gap has *widened* over the period, not narrowed.
- **The private-school advantage reversed in 2024**: private schools led in 2017 and 2021, then fell 3pp in 2024 while state government schools rose 5pp — the year structured, government-driven pedagogy (NIPUN Bharat) started catching up to resourcing.
- **Rural outperformed urban for the first time**, coinciding with targeted rural rollout of foundational literacy and numeracy (FLN) programs.
- **Maths fell harder than Language during COVID** (−7.6pp vs −4.7pp) — Language can be practiced informally at home; Maths generally needs structured, teacher-led practice.
- **Punjab: #28 → #1**. The clearest replicable success story in the data — a sustained SCERT-DIET partnership model with teacher-led data review cycles took Punjab from bottom-third to the top-ranked state in Language over 7 years.
- Language and Maths scores move together almost perfectly across states (r = 0.987) — no state outperforms nationally in one subject while lagging in the other, suggesting shared systemic drivers.

## Recommendations

The full write-up includes six data-grounded recommendations, including targeting the bottom 35% in Maths specifically (rather than extending existing FLN programs uniformly), replicating the Punjab model in lagging states, shifting from average-score to percentile-distribution reporting, and tying state NIPUN funding to SC/ST gap closure rather than overall averages.

## Data sources

- [nas.gov.in](https://nas.gov.in) — NCERT National Achievement Survey report cards
- [dashboard.parakh.ncert.gov.in](https://dashboard.parakh.ncert.gov.in) — PARAKH Rashtriya Sarvekshan dashboard
- NCERT NAS 2021 National Report, PARAKH PRS 2024 National Report

## Key assumptions & limitations

- NAS 2017 covered government and aided schools only; NAS 2021 and PRS 2024 added private schools, so direct comparison across all three rounds is approximate for school-management breakdowns.
- Only Grade 3 has a directly comparable testing format across all three rounds — Grade groupings changed under NEP 2020 (PRS 2024 tests Grades 3/6/9, versus NAS's 3/5/8/10), so no single cohort can be tracked longitudinally through this data.
- 2021 IRT-based scores are normalized (divided by 5) for comparability with the other rounds.

## Tech

A single self-contained HTML file — [D3.js](https://d3js.org/) and [Chart.js](https://www.chartjs.org/) loaded via CDN, no build step or server required.

## Author

Built by Ipsita Pal as an independent analysis project.
