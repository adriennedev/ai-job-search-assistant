# Connectors: the `~~category` placeholder convention

This plugin is written to work with whatever tools YOU have connected, not a specific product. Anywhere a skill needs an external tool, it names a **category** with a `~~` prefix instead of a brand:

| Placeholder | Meaning | Examples of what could fill it |
|---|---|---|
| `~~spreadsheet` | The spreadsheet where your job tracker lives | Google Sheets, Excel/OneDrive, Airtable, Notion database, a local .xlsx |
| `~~email` | How progress summaries reach you | Gmail, Outlook, any mail connector — or a saved Markdown file if none |
| `~~browser` | Browser automation for reading job postings | Claude in Chrome, or pasting posting text manually |
| `~~documents` | Where generated .docx files are saved | Local outputs folder, Google Drive, OneDrive |

## How it works at runtime

When Claude encounters `~~spreadsheet` in a skill, it should:

1. **Use the matching connected tool** if one is available in the session (e.g., a Google Sheets or Drive connector).
2. **Ask you once** which tool to use if several could match, then stay consistent for the session.
3. **Fall back gracefully** if nothing matches: save output as a local file (CSV for tracker rows, Markdown for the summary email) and tell you where it is. Never silently skip a step.

## Making it permanent

To hardcode your choices, edit the SKILL.md files and replace the placeholders with your actual tool and resource, e.g. replace `your job tracker in ~~spreadsheet` with `the Job_Tracker Google Sheet at <your-sheet-URL>`. See USER-INSTRUCTIONS.md.
