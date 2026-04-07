---
layout: page
title: Project Plan & Major Updates
description: Work plan and milestones for our classroom occupancy prediction project
img: assets/img/7.jpg
importance: 2
category: work
---

subtitle: <a href='#' style="font-weight:700; font-size:1.25rem;">5-Week Project Plan</a>

This schedule begins on **April 1, 2026**, with the **demo deadline on April 24, 2026** and the **final report deadline on May 3, 2026**.

### Week 1 (April 5–April 11, 2026): Sensor Bring-Up and Data Pipeline Foundation

- Integrate and calibrate the thermal sensor to reliably capture human movement and occupancy counts.
- Build an initial occupancy tracking pipeline, including timestamping, count extraction, and basic quality checks.
- Validate sensor placement and field of view in selected classrooms.
- Define a data schema for merging occupancy counts with class schedules, class sizes, weather, and FCE signals.
- **Milestone:** Produce the first end-to-end day of synchronized occupancy data.

### Week 2 (April 12–April 18, 2026): Baseline Modeling and Early Prototype for Demo

- Clean and preprocess collected data, including missing-interval handling, outlier checks, and feature generation.
- Train and evaluate the linear regression baseline for day-ahead occupancy forecasting.
- Train the proposed model on the same feature set and create initial comparison plots and tables using metrics such as MAE and RMSE.
- **Milestone:** Generate preliminary baseline-versus-proposed model results.

### Week 3 (April 19–April 24, 2026): Demo Hardening and Artifact Finalization

- Perform targeted error analysis by time of day, room type, and scheduled versus unscheduled usage.
- Improve model robustness and finalize the model version used for demo-day artifacts.
- Produce a poster draft with the problem statement, method diagram, sensor setup, and key preliminary results.
- **Milestone (April 24, 2026):** Present our findings during the demo.

### Week 4 (April 25–May 1, 2026): Report Completion and Final Experiments

- Run final experiments with locked train, validation, and test splits and finalize all results tables and figures.
- Expand the Method, Experiment, and Results sections with reproducible settings and clear metric definitions.
- Add discussion of limitations, deployment considerations, and future work.
- **Milestone:** Complete a near-final report draft.

### Week 5 (May 2–May 3, 2026): Final Edits and Submission

- Perform final proofreading, formatting, and consistency checks across the text, captions, and references.
- Verify that all reported numbers match the latest experiment outputs.
- Finalize the abstract and conclusion to reflect the final empirical findings.
- **Milestone (May 3, 2026):** Submit the final report.

## Notes

This page documents the planned progression of the project from sensor deployment through model development, demo preparation, and final report submission.
