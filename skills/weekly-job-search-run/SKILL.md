---
name: weekly-job-search-run
description: >
  Run the user's full weekly AI-augmented job search pipeline. Use when the user says
  "run the weekly job search", "check my saved jobs", "refresh my job pipeline", or when
  triggered by a scheduled task. Reviews job postings, updates the tracker in ~~spreadsheet,
  generates tailored resumes and cover letters, and sends a progress summary via ~~email.
  NEVER applies to jobs.
---

# Weekly Job Search Run

Execute the pipeline in order. Read the candidate profile and rubric below first.

## Hard guardrails (non-negotiable)

- NEVER click Apply or submit any application form. All output stops at "ready for the user to review."
- NEVER message recruiters or post publicly.
- Log negative outcomes honestly in the tracker.

## Your candidate profile (user: fill this in — see USER-INSTRUCTIONS.md)

- **Target roles:** [list target job titles]
- **Avoid:** [hard-blocker titles/requirements, e.g., roles requiring skills you don't have]
- **Location policy:** [remote? hybrid metro? travel tolerance?]
- **Strengths:** [5-8 evidence-backed selling points with numbers]
- **Weaknesses to manage:** [real gaps + honest reframes]
- **Voice notes for cover letters:** [phrases, beliefs, stories in your own words]
- **Contact block:** [City, State | phone | email | LinkedIn URL]

## Fit-scoring rubric (1-10) — user: tune the bonuses/penalties

Start at 5, then:
- +2 role matches your primary target category with no hard-blocker requirements
- +1 strong domain overlap with your background
- +1 posting explicitly values a differentiator you have
- +1 work style matches (e.g., client-facing, IC, leadership — whichever fits you)
- -1 heavy screen on a tool/skill you lack but could learn
- -2 niche domain bar far from your experience
- -3 or more: hard blocker (a must-have you don't have and won't claim)
Cap at 3 if any hard blocker exists. Never tailor materials for scores <= 3.

## Pipeline

### 1. Gather jobs (~~browser)
- Read the user's saved jobs page on their job board.
- Search for postings from the past week matching the target roles above.
- For each candidate job capture: title, company, URL, salary, requirements, remote policy, applicant volume, posted date.

### 2. Filter
- Drop anything no longer accepting applications.
- Apply the location policy. Borderline locations pass only if fit score >= 8.
- Flag hard blockers; score <= 3, do not tailor materials.

### 3. Score and update tracker
- Score each job with the rubric.
- Open the tracker in ~~spreadsheet. Add new rows to the Tracker tab (never overwrite existing rows). Read Status and Recruiter Feedback for jobs already applied to.

### 4. Learn from outcomes
- Compare observed interview rate to the user's assumed rate (Model tab if present).
- Identify patterns in no-response rows: title screens, missing keywords, miscalibrated scores.
- Adjust this week's targeting and note the adjustment in the summary.

### 5. Generate materials
- For up to 3 new jobs scoring >= 7, create a tailored resume + cover letter via the `tailor-application` skill. Save to ~~documents.

### 6. Deliver summary (~~email)
Send to the user's address only:
- New jobs, scores, which got tailored materials (attached or linked)
- Status changes and feedback since last run
- Observed vs. expected interview rate
- 2-3 concrete suggestions (referral paths, profile keywords, certifications)
- Link to the tracker

### 7. Self-review
If scoring weights or filters no longer match observed results, propose specific edits to this skill and ask the user to approve them.
