# How to Start a New Project

5 steps. Takes 10 minutes.

---

## Step 1: Fork This Template

1. Go to: https://github.com/vishalm111296-commits/ai-brain-os
2. Tap: Use this template → Create a new repository
3. Name it your project:
   - three-slap-research
   - youtube-system
   - business-plan
   - fitness-tracker
4. Set to Public
5. Tap: Create repository

All files and prompts copy automatically.

---

## Step 2: Fill in PROJECT_BRIEF.md (Most Important)

Open PROJECT_BRIEF.md.
Answer these 4 questions:
- What is this project?
- Why are we doing it?
- How will we know it worked? (with numbers)
- How will we know it failed? (with numbers)

Commit.

---

## Step 3: Fill in BRAIN.md

Open BRAIN.md.
Fill in:
- Current goal (one sentence)
- Blocker (or write: none)
- Best hypothesis (your best guess right now)
- Next action (the very first task)

Commit.

---

## Step 4: Update Phone Notes (One Change Only)

Open Google Keep → open your START note.
Replace every occurrence of:
  ai-brain-os
With:
  your-new-repo-name

Example:
OLD: https://raw.githubusercontent.com/vishalm111296-commits/ai-brain-os/main/BRAIN.md
NEW: https://raw.githubusercontent.com/vishalm111296-commits/three-slap-research/main/BRAIN.md

Nothing else changes. Same prompts. Same rules. Just the repo name.

---

## Step 5: Run First Session

Open any AI.
Paste START note.
Change last line to your first task.
AI reads files → outputs UNDERSTANDING CHECK → you confirm → work begins.

---

## Where Every Type of AI Output Goes

| What AI generates | Where it goes | Rule |
|---|---|---|
| Code, Python scripts | code/ folder | Save dated + overwrite latest.py |
| Experiment numbers | RESULTS.csv | Append new row |
| Confirmed observations | FACTS.md | Append new line |
| Choices and reasoning | DECISIONS.md | Append new block |
| Rejected ideas | DO_NOT_REPEAT.md | Append one line |
| Current status | BRAIN.md | Overwrite |
| Stop point | CHECKPOINT.md | Overwrite |
| Session log | sessions/ folder | New dated file, never overwrite |
| Weekly digest | WEEKLY_SUMMARY.md | Overwrite |

---

## Daily vs Weekly vs Occasional

### Every Session (phone, 3 minutes total)
- Commit updated BRAIN.md
- Commit updated CHECKPOINT.md
- Append new rows to RESULTS.csv if experiments ran

### Every Week (Sunday, 10 minutes)
- Append to DO_NOT_REPEAT.md
- Overwrite RED_TEAM.md
- Overwrite WEEKLY_SUMMARY.md using compress.md prompt

### Occasionally (when relevant)
- Add to FACTS.md after confirmed observations
- Add to DECISIONS.md after major choices
- Update VALIDATION.md if checklist changes
- Update SPEC.md if project scope changes

---

## When Tokens Run Out Mid-Task

1. Every AI response ends with a RESUME BLOCK automatically
2. Find the last complete response — copy the resume block at the bottom
3. Open new account or new model
4. Paste prompts/resume.md
5. Replace links with your repo's raw links
6. AI reads MASTER_PROMPT + BRAIN + CHECKPOINT
7. AI outputs UNDERSTANDING CHECK
8. You confirm
9. Work continues from exact step

No re-explaining. No starting over.
