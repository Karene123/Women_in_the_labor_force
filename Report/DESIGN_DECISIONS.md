# DESIGN_DECISIONS.md
# WBL Trajectory Analysis — Methodological Decision Log
# Created: Day 1
# Format: Each entry is labelled DD-XXX.
# Rule: Never delete entries — only append.

---

## DD-000c — Differentiation from Hernández-Lara et al. (2025)

**What they did:**
Hernández-Lara et al. (2025) perform longitudinal analysis of WBL scores
grouped by income level, region, and performance tier. They describe how
trajectories differ across these predefined categories and identify leading
vs lagging economies within those groups.

**What they did not do:**
They do not apply an unsupervised distance-based clustering algorithm to the
raw WBL time series. Their groupings are imposed using existing World Bank
classifications, not discovered from the data. They do not use DTW, do not
compute a trajectory distance matrix, and do not apply SHAP to explain
cluster membership.

**How this project differs:**
This project uses Dynamic Time Warping over the full 1971–2024 WBL panel to
algorithmically identify economies that share reform trajectories regardless
of their income group or region. Cluster membership is then explained using
SHAP applied to a trained classifier — making the explanatory layer
data-driven rather than descriptive.

---

## DD-001 — Filtering aggregates from the WBL panel

**Decision:** Removed World Bank aggregate rows, kept only real economies.

**Method:** Used wbgapi aggregate flag (e.get('aggregate', False)).

**Result before filtering:** 266 rows (217 economies + 49 aggregates)
**Result after filtering:**  217 economies, 55 years (YR1971-YR2025)

**Saved to:** data/processed/wbl_clean.csv

---

