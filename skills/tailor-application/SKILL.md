---
name: tailor-application
description: >
  Generate a tailored resume and cover letter (.docx) for one specific job posting.
  Use when the user says "tailor my resume for this job", "write a cover letter for X",
  "prep application materials", or pastes a job posting URL or description.
---

# Tailor Application

Produce one resume + one cover letter as .docx files, tailored to a single posting.

## Steps

1. Read the job posting (URL via ~~browser, or pasted text). Extract: must-have requirements, repeated keywords, mission language, compensation, team context.
2. Read the candidate profile in `../weekly-job-search-run/SKILL.md` (rubric, strengths, weaknesses, voice notes, contact block). If the profile section is still blank, stop and ask the user to complete it per USER-INSTRUCTIONS.md.
3. **Resume:** start from the user's base resume (or the closest previously tailored version in ~~documents). Adjust the Summary, reorder Core Skills to mirror the posting's language, and select experience bullets that map to the top responsibilities. Keep history strictly factual — never invent employers, titles, dates, or credentials.
4. **Cover letter:** one page, 4 paragraphs —
   (a) hook tying the user's direction to the role,
   (b) proof from career history with numbers,
   (c) the user's differentiator story (from voice notes),
   (d) honest gap acknowledgment reframed as a fast-learning pattern, plus a call to action.
   Write in the user's voice per their voice notes: direct, warm, evidence-first, no buzzword soup.
5. **Honesty rule:** name one real gap plainly. Hiring managers trust candidates who self-assess accurately.
6. Save as `Resume_<Name>_<Company>_<Role>.docx` and `CoverLetter_<Name>_<Company>_<Role>.docx` in ~~documents. Record the version name in the tracker row (~~spreadsheet).
7. Never submit anything. Deliver files for the user's review.
