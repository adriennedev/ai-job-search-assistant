---
name: update-job-tracker
description: >
  Update the job tracker in ~~spreadsheet with statuses, outcomes, feedback, and test
  notes, and recalibrate expectations. Use when the user says "update the tracker",
  "log an interview", "I got rejected by X", "mark X applied", or "how are my odds looking".
---

# Update Job Tracker

The tracker lives in ~~spreadsheet (the user's job tracker — see USER-INSTRUCTIONS.md for the expected columns).

## Steps

1. Open the Tracker tab. Find the row by company + title; add a row if missing (match existing column formats; Status values: Applied | No Response | Interview | Offer | Rejected).
2. Set Status, Date Applied, Test Notes (what was varied: resume version, referral, timing), and Recruiter Feedback verbatim where available.
3. If a Model tab exists: once n >= 15 applications, compare the observed interview rate to the assumed callback rate and tell the user whether the assumption should be raised or lowered. The user edits the assumption cells themselves.
4. Report back: current funnel counts (applied / no-response / interview / offer), observed rates, and one pattern worth acting on (e.g., "postings with <50 applicants are converting 3x better").
5. Never fabricate outcomes. If data is ambiguous, ask the user.
6. Never delete or overwrite rows the user wrote; only append or fill the specific cells being updated.
