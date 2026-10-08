# Boliyo / Delivery Health Tracker — Phase 2 Analysis

**Participants:** 8 | **Sessions conducted:** 8 × 3 tasks = 24 observations | **Date analysed:** 2026-10-08

---

## 1. Completion Rate & Median Time per Task

| Task | Completed | Completion Rate | Median Time (completers only) |
|---|---|---|---|
| T1 — Log a Health Entry | 8 / 8 | **100%** | **48.5 s** |
| T2 — View Trend Summary | 6 / 8 | **75%** | **70.0 s** |
| T3 — Update a Profile Detail | 7 / 8 | **87.5%** | **58.0 s** |

> **Methodology notes**
> - Completion = reached success condition without facilitator help.
> - Median time is calculated over **completers only**; including failed sessions would inflate times artificially.
> - T1 median: average of 4th & 5th sorted value (46 s, 51 s) = 48.5 s.
> - T2 completers (n=6): 61, 66, 68, 72, 79, 88 → median = (68+72)/2 = 70.0 s.
> - T3 completers (n=7): 49, 52, 55, 58, 63, 69, 73 → median = 4th value = 58.0 s.

---

## 2. Issue Themes — Ranked by Severity × Frequency

**Scoring formula:** `avg_severity × affected_participant_count`
(Severity: 1 = cosmetic, 2 = causes delay, 3 = blocks task)

### Theme 1 — Filter Discoverability (Task 2) 🔴
**Score: 10.0** | Affected: 4 / 8 participants | **2 task failures (P02, P06)**

| Participant | Severity | Errors | Quote |
|---|---|---|---|
| P01 | 2 | 1 | "I had to look around before finding the delayed orders." |
| P02 | 3 | 2 | "I wasn't sure which filter showed delayed deliveries." |
| P04 | 2 | 2 | "I clicked the wrong filter first." |
| P06 | 3 | 2 | "The filter options weren't obvious." |

**Pattern:** Participants could not locate or interpret the filter controls for delayed/health-category views. Two participants gave up entirely. Even completers took a detour (avg 2 errors in this group vs. 0 for successful Task 1 completers).

---

### Theme 2 — Unclear Call-to-Action / Next Step (Task 3) 🟠
**Score: 7.0** | Affected: 3 / 8 participants | **1 task failure (P04)**

| Participant | Severity | Errors | Quote |
|---|---|---|---|
| P02 | 2 | 1 | "I understood the information after exploring." |
| P04 | 3 | 3 | "I couldn't tell what action I was supposed to take." |
| P08 | 2 | 1 | "I would like a clearer next action." |

**Pattern:** Once on the dashboard/summary screen, participants did not know what to do next. P04 exhausted all visible options before failing. P02 and P08 completed but only after unnecessary exploration.

---

### Theme 3 — Navigation Entry Point / Initial Orientation (Task 1) 🟡
**Score: 6.0** | Affected: 3 / 8 participants | **0 failures**

| Participant | Severity | Errors | Quote |
|---|---|---|---|
| P02 | 2 | 1 | "I expected the status to be at the top." |
| P04 | 2 | 1 | "The labels were slightly confusing." |
| P06 | 2 | 1 | "I wasn't immediately sure where to start." |

**Pattern:** First-glance orientation is slightly off. Users complete the task but need a scanning phase first. Task is still 100% successful, so this is a speed / confidence issue rather than a failure driver.

---

### Theme 4 — Category Label Comprehension (Task 2) 🟡
**Score: 4.0** | Affected: 2 / 8 participants | **0 failures**

| Participant | Severity | Errors | Quote |
|---|---|---|---|
| P05 | 2 | 1 | "It took a moment to understand the delivery health categories." |
| P08 | 2 | 1 | "The delivery health categories could be explained better." |

**Pattern:** The naming/labelling of health category buckets is not immediately self-explanatory. Participants figure it out but without confidence.

---

### Theme 5 — Visual Richness of Summary (Task 3) ⚪
**Score: 1.0** | Affected: 1 / 8 participants | **0 failures**

| Participant | Severity | Errors | Quote |
|---|---|---|---|
| P01 | 1 | 1 | "The summary makes sense but could be more visual." |

**Pattern:** Low-frequency, cosmetic. P01 understood the data fine; this is a polish request, not a usability problem.

---

## 3. Top 2 Highest-Impact Fixes

### Fix 1 — Redesign the filter control for delayed/health-category views
**Rationale:** Filters are the single biggest failure driver — 2 outright failures, 2 delayed completions, worst average severity (2.5). Making the filter label explicit (e.g., rename to "Delayed Orders" rather than a generic filter icon) and surfacing it above the fold would directly attack the 25% non-completion rate on Task 2.

### Fix 2 — Add a visible, labelled primary action on the dashboard summary screen
**Rationale:** 3 of 8 participants (including 1 failure) did not know what to do after landing on the summary view. A single prominent CTA (e.g., "View delayed orders →" or "Take action") costs minimal development effort and directly addresses both Theme 2 failures and the residual confusion in Theme 3.

---

## 4. What to Leave for Later

- **Category label comprehension (Theme 4):** Real problem, but lower frequency and no failures. A tooltip or one-line explainer would suffice — lower effort than a filter redesign.
- **Visual richness (Theme 5):** Single participant, cosmetic. Defer to a polish sprint.
- **Initial orientation (Theme 3):** Task 1 is already 100% complete. Minor label or hierarchy tweaks post-Fix 1 & 2.

---

*Analysis based on 8 participants, 24 task observations. Sample is small — findings are directional. Prioritise fixes that address outright failures (Themes 1 & 2) before drawing conclusions about subtler patterns.*
