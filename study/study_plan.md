# Boliyo / Delivery Health Tracker — Usability Study Plan

---

## Study Goal

Identify usability barriers that prevent delivery workers from successfully logging and reviewing their health data within a single session, so the team can prioritise the highest-impact fixes before the next release.

---

## Research Questions

1. **Task success & efficiency** — Can participants complete the three core workflows (log a health entry, view their trend summary, update a personal profile detail) without assistance, and how long does each task take?
2. **Comprehension & labelling** — Do the labels, icons, and data visualisations communicate their meaning clearly, or do participants misread or hesitate over them?
3. **Trust & motivation** — Do participants feel the app gives them actionable, trustworthy information about their health, or does it feel confusing / irrelevant to their daily delivery work?

---

## Participant Criteria

| Criterion | Requirement |
|---|---|
| Occupation | Active delivery worker (any platform: food, parcel, grocery) |
| Device | Uses a smartphone daily (Android or iOS) |
| App experience | Has **not** used Boliyo before (fresh perspective) |
| Health interest | No requirement — any level of engagement with personal health |
| Accessibility | Comfortable giving verbal feedback in the session language |
| Exclusion | Do **not** recruit team members, beta testers, or people who have seen the app's marketing |

**Target:** 5–8 participants. Aim for at least 2 different delivery platforms and a mix of experience levels (< 1 year / 1–3 years / 3 + years on the job).

---

## 15-Minute Session Script

> **Facilitator notes (do not read aloud):**
> - Run sessions 1-on-1. Remote or in-person both work.
> - Use the participant's own phone if possible; otherwise a test device pre-loaded with the app.
> - Keep the app reset to a blank/demo account before each session.
> - Fill `session_log.csv` live or immediately after — never from memory hours later.
> - Your role is to observe, not to help. If a participant asks "Is this right?", reply: *"What would you expect to happen?"*

---

### ① Intro & Warm-Up [~2 min]

> *"Thanks for joining me today. My name is [your name]. I'm going to ask you to try out an app while thinking aloud — meaning, please say whatever is going through your mind as you go. There are no right or wrong answers; we're testing the app, not you. I can't answer questions about how the app works during the tasks, but feel free to ask anything else. We'll be here for about 15 minutes. Do you have any questions before we start?"*

Warm-up question (answer is not logged):

> *"Can you tell me a little about your delivery work — what platform, how many shifts a week, roughly?"*

---

### ② Task Block [~10 min total]

Hand the participant the relevant **task card** (see `task_cards.md`) for each task. Read the task aloud as you hand it over.

**Think-aloud prompts to use if the participant goes silent (> ~10 seconds):**

- *"What are you looking at right now?"*
- *"What are you expecting to happen when you tap that?"*
- *"What would you do next if you weren't sure?"*
- *"How does this feel compared to what you expected?"*

**Task 1 — Log a Health Entry** [~3 min]
**Task 2 — View a Health Trend Summary** [~3 min]
**Task 3 — Update a Profile Detail** [~4 min]

After each task, note in `session_log.csv`:
- `completed` (Y/N — did they reach the success condition without facilitator help?)
- `time_seconds` (start the moment you finish reading the task card)
- `errors` (count of wrong taps, wrong screens, or visible confusion moments)
- `quote` (the most revealing verbatim thing they said)
- `severity` (1 = cosmetic/minor, 2 = causes delay, 3 = blocks task)

---

### ③ Closing Questions [~3 min]

Ask these after all three tasks. Do not correct misunderstandings — just listen.

1. *"If you had a magic wand, what's the one thing you'd change about the app right now?"*
2. *"Was there any moment where you weren't sure what to do next? What did that feel like?"*
3. *"Would you use an app like this during or after your delivery shifts? Why or why not?"*
4. *"On a scale of 1–10, how easy did the app feel overall? What would make it a 10?"*

Close with:

> *"Thank you so much — your feedback is genuinely helpful. Everything you told me goes directly to improving the app. Do you have any questions for me?"*

---

## Logistics Checklist

- [ ] Consent note signed / verbally agreed before session starts
- [ ] Test device / participant device app reset to blank state
- [ ] `session_log.csv` template open and ready
- [ ] Task cards printed or on a separate screen
- [ ] Timer ready (phone stopwatch is fine)
- [ ] Note any environmental factors that might affect results (noisy location, interrupted session, etc.) in the `errors` or `quote` field with a `[NOTE]` prefix
