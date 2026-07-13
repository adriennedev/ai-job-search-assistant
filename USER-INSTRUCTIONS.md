# User Instructions — customize before first use

This is a **template**. It ships with blanks where your personal information goes. Complete these steps before running any skill.

## 1. Fill in your candidate profile (required)

Open `skills/weekly-job-search-run/SKILL.md` and complete the **"Your candidate profile"** section:

- **Target roles** — job titles you want (e.g., "Product Manager", "Data Analyst").
- **Avoid** — titles or requirements that are hard blockers for you.
- **Location policy** — remote only? Which metro for hybrid/onsite? Travel tolerance?
- **Strengths** — 5-8 concrete, evidence-backed selling points (years of experience, budgets managed, named projects, public proof of work).
- **Weaknesses to manage** — real gaps and the honest reframe for each.
- **Voice notes** — 3-5 phrases, beliefs, or stories that make cover letters sound like you.
- **Contact block** — city, phone, email, LinkedIn URL (used in generated resumes).

## 2. Tune the fit rubric (recommended)

The rubric in `weekly-job-search-run/SKILL.md` starts every job at 5/10 and adds/subtracts points. Edit the bonus and penalty lines to match what actually predicts fit for you. Keep the "cap at 3 if a hard blocker exists" rule.

## 3. Set up your tracker spreadsheet

Create a spreadsheet (any tool — see CONNECTORS.md) with a **Tracker** tab containing at least: Company, Title, URL, Date Found, Fit Score, Status (Applied | No Response | Interview | Offer | Rejected), Date Applied, Resume Version, Test Notes, Recruiter Feedback. Optionally add a **Model** tab with your assumed callback rate so the skills can compare observed vs. expected results. Then tell Claude where the tracker lives (or hardcode the link in the skills).

## 4. Point the skills at your job sources

`weekly-job-search-run` Step 1 lists search queries and a saved-jobs page. Replace the example queries with your target titles and set the job board(s) you actually use (LinkedIn, Indeed, Otta, company boards).

## 5. Set your delivery email

Replace `~~email` behavior by telling Claude your address once, or hardcode it in Step 6 of `weekly-job-search-run/SKILL.md`.

## 6. Provide a base resume

Put your current resume (.docx or text) in a folder Claude can read, and tell Claude where it is. `tailor-application` starts from it and never invents facts.

## Optional

- Schedule the weekly run (e.g., every Wednesday morning) with your client's scheduled-tasks feature.
- After ~15 applications, ask Claude to compare observed interview rates to your assumptions and recalibrate the rubric.

## What you should never change

The guardrails: the plugin must never apply to jobs, message recruiters, or fabricate outcomes. Those lines exist so an automated pipeline can't act on your behalf.
