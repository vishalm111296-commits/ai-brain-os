# How to Start a New Project

5 steps. Takes 10 minutes.

---

## Step 1: Fork This Template

1. Go to: https://github.com/vishalm111296-commits/ai-brain-os
2. Tap the green button: Use this template
3. Tap: Create a new repository
4. Name it your project:
   - three-slap-research
   - youtube-system
   - business-plan
   - fitness-tracker
5. Set to Public
6. Tap: Create repository

All 10 files and all prompts are copied automatically.

---

## Step 2: Fill in SPEC.md

Open SPEC.md in your new repo.
Answer these 4 questions:
- What are we building?
- What does success look like (with numbers)?
- What tools and data do we have?
- What are the rules we cannot break?

Commit the file.

---

## Step 3: Fill in BRAIN.md

Open BRAIN.md.
Fill in:
- Current goal (one sentence)
- Blocker (or write none)
- Best hypothesis (your best guess right now)
- Next action (the very first task)

Commit the file.

---

## Step 4: Update Your Phone Notes

Open Google Keep.
Open your START note.
Change every link that says ai-brain-os to your new repo name.

Example:
OLD: https://raw.githubusercontent.com/vishalm111296-commits/ai-brain-os/main/BRAIN.md
NEW: https://raw.githubusercontent.com/vishalm111296-commits/three-slap-research/main/BRAIN.md

Change only the repo name. Everything else stays the same.

---

## Step 5: Run First Session

Open any AI.
Paste your START note.
Change the last line to your first task.
Start working.

---

## Where Each Type of AI Output Goes

| What AI generates | Where it goes | Rule |
|---|---|---|
| Python code or scripts | code/ folder | Save dated + overwrite latest.py |
| Experiment numbers | RESULTS.csv | Append new row |
| Confirmed observations | FACTS.md | Append new line |
| Choices and why | DECISIONS.md | Append new block |
| Rejected ideas | DO_NOT_REPEAT.md | Append new line |
| Current status | BRAIN.md | Overwrite |
| Stop point | CHECKPOINT.md | Overwrite |
| Session log | sessions/ folder | New dated file |
| Weekly digest | WEEKLY_SUMMARY.md | Overwrite |

---

## When Tokens Run Out Mid-Task

1. AI always ends every response with a RESUME BLOCK
2. Copy the resume block
3. Open DO_NOT_REPEAT.md in GitHub — paste latest CHECKPOINT content
4. Switch to new account or model
5. Paste the RESUME prompt from prompts/resume.md
6. Add the raw GitHub links
7. New AI reads files and continues from exact step

No re-explaining. No starting over. Zero work lost.
