# AI Job Search Assistant

A Claude plugin that runs an AI-augmented job search pipeline: it reviews job postings, scores them against a fit rubric you define, keeps a tracker spreadsheet up to date, generates tailored resumes and cover letters, and emails you a weekly progress summary.

## The hard rule

**This plugin NEVER applies to jobs on your behalf.** It never clicks Apply, never submits forms, never messages recruiters, never posts publicly. Every deliverable stops at "ready for your review." You stay in control of every application.

## Skills

- **weekly-job-search-run** — the full weekly pipeline: gather saved and new postings, filter by your criteria, score fit 1-10 against your rubric, update your tracker in ~~spreadsheet, generate tailored materials for top targets, learn from prior outcomes, and send a summary via ~~email.
- **tailor-application** — generate a tailored resume + cover letter (.docx) for a single job posting.
- **update-job-tracker** — log statuses, outcomes, recruiter feedback, and test notes in your tracker, and report funnel stats.

## Principles

1. Never submit an application on the user's behalf. Deliverables stop at "ready for review."
2. Log outcomes honestly — failed applications are data, not embarrassments.
3. "Hours saved" is not the success metric; interview rate, output quality, and reproducibility are.
4. Never invent employers, titles, dates, credentials, or outcomes.

## Example use cases

- **Example 1:** "Run the weekly job search" — Claude reviews your saved jobs and new postings, scores each against your rubric, adds them to your tracker, drafts tailored materials for the top 3, and emails you a summary with suggestions.
- **Example 2:** "Tailor my resume for this posting: [URL]" — Claude reads the posting, mirrors its language in your resume summary and skills, writes a 4-paragraph cover letter in your voice, and saves both as .docx for your review.
- **Example 3:** "I got an interview at Acme, update the tracker" — Claude logs the status change, updates the funnel counts, and tells you which pattern in your data is worth acting on.

## Setup

Read **USER-INSTRUCTIONS.md** (what to customize before first use) and **CONNECTORS.md** (how the `~~category` tool placeholders work). You must fill in your candidate profile and fit rubric before the scoring skills are useful.
