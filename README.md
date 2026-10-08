# Boliyo / Delivery Health Tracker — Usability Study

A complete, end-to-end usability study kit and analysis for **Boliyo**, a delivery health tracking app. The study was conducted across three phases: kit creation, initial analysis, and post-fix validation.

---

## Study Overview

| | |
|---|---|
| **App** | Boliyo / Delivery Health Tracker |
| **Method** | Moderated think-aloud usability sessions |
| **Phase 2 participants** | 8 (P01–P08) |
| **Phase 3 participants** | 5 (P09–P13) |
| **Session length** | ~15 minutes each |
| **Tasks per session** | 3 |

---

## Results Summary

### Completion Rate

| Task | Before Fixes | After Fixes |
|---|---|---|
| T1 — Log a Health Entry | 100% | 100% |
| T2 — View Trend Summary | 75% ❌ | **100%** ✅ |
| T3 — Update a Profile Detail | 87.5% ❌ | **100%** ✅ |
| **Overall** | **88%** | **100%** |

### Median Time (completers only)

| Task | Before | After | Change |
|---|---|---|---|
| T1 | 48.5 s | 43.0 s | ▼ −11% |
| T2 | 70.0 s | 51.0 s | ▼ −27% |
| T3 | 58.0 s | 49.0 s | ▼ −16% |

---

## Top Issues Found & Fixed

| Priority | Issue | Fix Applied |
|---|---|---|
| 🔴 #1 | Filter control for delayed orders was not discoverable — 2 task failures | Renamed to "Delayed Orders", surfaced above the fold |
| 🟠 #2 | Dashboard summary had no clear call-to-action — 1 task failure | Added a labelled primary CTA button |

---

## Repository Structure

```
study/
├── study_plan.md        # Goal, research questions, participant criteria, 15-min session script
├── task_cards.md        # 3 task cards with success conditions
├── session_log.csv      # Data log template + filled study data
├── consent_note.md      # Plain-language participant consent text
├── phase2_analysis.md   # Phase 2: completion rates, issue themes, top 2 fix recommendations
└── before_after.md      # Phase 3: before/after metrics side by side
```

---

## How to Reuse This Kit

1. Reset the app to a blank/demo account before each session.
2. Read `consent_note.md` to the participant and get verbal agreement.
3. Follow the script in `study_plan.md` (intro → 3 tasks → closing questions).
4. Hand participants the relevant card from `task_cards.md` one at a time.
5. Fill `session_log.csv` live or immediately after each session.
6. Paste filled CSV to your analyst to generate `phase2_analysis.md`.

---

## Sample Size Caveat

> Both rounds used small samples (n=8 and n=5). All findings are **directional, not statistically conclusive**. For higher confidence, run a third round with 8–10 new participants or conduct an unmoderated remote study.

---

*Study conducted: October 2026*
