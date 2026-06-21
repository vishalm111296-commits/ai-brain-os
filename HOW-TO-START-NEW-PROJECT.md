# How to Start a New Project

Pick any one of the 3 methods below.
All 3 give you the same result.

---

## Method 1 — Fork (Fastest, 2 minutes)

1. Go to: https://github.com/vishalm111296-commits/ai-brain-os
2. Tap the **Fork** button (top right)
3. Change the repository name to your project:
   - home-loan-os
   - three-slap-research
   - youtube-system
   - fitness-tracker
4. Tap **Create fork**

Done. All files copied to your account automatically.
Your new repo: github.com/YOUR-USERNAME/your-project-name

---

## Method 2 — AI Bulk Copy (No GitHub needed, 5 minutes)

If forking feels complicated, let AI create all files for you.

Open any AI. Paste this prompt:

```
I am starting a new project called: [YOUR PROJECT NAME]

Create all of these files ready to paste into a new GitHub repo:

1. PROJECT_BRIEF.md — using this project: [DESCRIBE YOUR PROJECT]
2. BRAIN.md — starter content for this project
3. CHECKPOINT.md — blank starter
4. RESULTS.csv — with correct headers only
5. DO_NOT_REPEAT.md — blank starter with table headers
6. SPEC.md — technical rules for this project

For each file:
- Output filename as header
- Output complete file content below it
- Keep every file under 200 words
```

AI outputs all 6 files.
Create a new GitHub repo (blank).
Create each file manually → paste content → commit.
6 files. 5 minutes.

Then copy these files from ai-brain-os (they never change):
- MASTER_PROMPT.md
- VALIDATION.md
- RED_TEAM.md
- ASSETS.md
- DISCOVERIES.md
- FACTS.md
- DECISIONS.md
- WEEKLY_SUMMARY.md
- All files in prompts/ folder

Open each file at:
https://github.com/vishalm111296-commits/ai-brain-os
Tap the file → tap Raw → copy everything → paste into your new repo.

---

## Method 3 — Manual Copy (Phone friendly, 10 minutes)

The simplest method. No forking. No AI needed.

1. Create a new blank repo on GitHub
   - Go to github.com → tap + → New repository
   - Name it your project
   - Set to Public
   - Do NOT initialize with README
   - Tap Create repository

2. Copy these files one by one from ai-brain-os:
   https://github.com/vishalm111296-commits/ai-brain-os

   For each file:
   - Tap the file name
   - Tap Raw
   - Select all → copy
   - Go to your new repo
   - Tap Add file → Create new file
   - Type the filename exactly
   - Paste content
   - Tap Commit

3. Copy in this priority order:

   Must copy first (edit these for your project):
   - PROJECT_BRIEF.md
   - BRAIN.md
   - CHECKPOINT.md
   - RESULTS.csv
   - SPEC.md

   Copy as-is (never change these):
   - MASTER_PROMPT.md
   - DO_NOT_REPEAT.md
   - ASSETS.md
   - DISCOVERIES.md
   - FACTS.md
   - DECISIONS.md
   - RED_TEAM.md
   - VALIDATION.md
   - WEEKLY_SUMMARY.md
   - prompts/startup.md
   - prompts/resume.md
   - prompts/end-session.md
   - prompts/generate-brief.md
   - prompts/generate-all-files.md

---

## After Any Method — 2 Things To Do

### Thing 1: Fill PROJECT_BRIEF.md for your project

Open PROJECT_BRIEF.md in your new repo.
Tap pencil.
Replace the template content with your project.

Fastest way: use the generate-brief.md prompt.
Open any AI → paste that prompt → change last line → get your brief → paste → commit.

### Thing 2: Update your Google Keep START note

Open Google Keep → open AI START note.
Replace every occurrence of:
  vishalm111296-commits/ai-brain-os
With:
  YOUR-USERNAME/your-new-repo-name

Example:
OLD: https://raw.githubusercontent.com/vishalm111296-commits/ai-brain-os/main/BRAIN.md
NEW: https://raw.githubusercontent.com/YOUR-USERNAME/home-loan-os/main/BRAIN.md

Nothing else changes. Done.

---

## Where Every Type of AI Output Goes

| What AI generates | Where it goes | Rule |
|---|---|---|
| Code, Python scripts | code/ folder | Save dated + overwrite latest.py |
| Experiment numbers | RESULTS.csv | Append new row |
| Confirmed observations | FACTS.md | Append |
| Choices and reasoning | DECISIONS.md | Append |
| Rejected ideas | DO_NOT_REPEAT.md | Append one line |
| Current status | BRAIN.md | Overwrite |
| Stop point | CHECKPOINT.md | Overwrite |
| Session log | sessions/ folder | New dated file |
| Weekly digest | WEEKLY_SUMMARY.md | Overwrite |
| Reusable assets 8+ | ASSETS.md | Append |

---

## Daily vs Weekly vs Occasional

### Every Session (3 minutes)
- Commit updated BRAIN.md
- Commit updated CHECKPOINT.md
- Append RESULTS.csv rows if experiments ran

### Every Sunday (10 minutes)
- Overwrite RED_TEAM.md using red-team prompt
- Overwrite WEEKLY_SUMMARY.md using compress prompt
- Append DO_NOT_REPEAT.md if anything was rejected

### Occasionally
- FACTS.md after confirmed observations
- DECISIONS.md after major choices
- ASSETS.md when AI flags importance 8+
- SPEC.md if project scope changes

---

## When Tokens Run Out Mid-Task

1. Every AI response ends with a RESUME BLOCK automatically
2. Copy the RESUME BLOCK from the last complete response
3. Open new account or new AI
4. Paste AI RESUME note from Google Keep
5. AI reads MASTER_PROMPT + BRAIN + CHECKPOINT
6. AI outputs UNDERSTANDING CHECK
7. You type: confirmed
8. Work continues from exact step

No re-explaining. No starting over.
