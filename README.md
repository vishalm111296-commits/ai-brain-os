# AI Brain OS — Universal Project Template

This is your reusable operating system for any AI-assisted project.

**GitHub = Brain. AI = Worker. Notes App = Launcher.**

---

## How to Use This Template

1. Fork this repo
2. Rename it to your project (example: `three-slap-research`)
3. Fill in `SPEC.md` with what you are building
4. Fill in `BRAIN.md` with current reality
5. Save the startup prompt in Google Keep
6. Start working

---

## File Index (Read Order for New AI)

| Order | File | Purpose |
|---|---|---|
| 1 | `SPEC.md` | What are we building? |
| 2 | `BRAIN.md` | What is true right now? |
| 3 | `CHECKPOINT.md` | Where did work stop? |
| 4 | `RESULTS.csv` | What did experiments show? |
| 5 | `DO_NOT_REPEAT.md` | What is permanently rejected? |
| 6 | `VALIDATION.md` | Checklist before trusting results |
| 7 | `FACTS.md` | Raw confirmed observations |
| 8 | `DECISIONS.md` | Why did we choose something? |
| 9 | `RED_TEAM.md` | Why might this project fail? |
| 10 | `WEEKLY_SUMMARY.md` | Compressed knowledge |

---

## File Rules

| File | Action When AI Updates It |
|---|---|
| `BRAIN.md` | OVERWRITE (always current) |
| `CHECKPOINT.md` | OVERWRITE (always current) |
| `RESULTS.csv` | APPEND new rows |
| `DO_NOT_REPEAT.md` | APPEND new lines |
| `DECISIONS.md` | APPEND new blocks |
| `FACTS.md` | APPEND new facts |
| `SPEC.md` | OVERWRITE only when project definition changes |
| `VALIDATION.md` | OVERWRITE only when checklist changes |
| `RED_TEAM.md` | OVERWRITE weekly |
| `WEEKLY_SUMMARY.md` | OVERWRITE every Sunday |

---

## Startup Prompt (Save in Google Keep)

```
Read these files before starting:
SPEC: [raw link]
BRAIN: [raw link]
CHECKPOINT: [raw link]
RESULTS: [raw link]
DO_NOT_REPEAT: [raw link]

Rules:
- Break task into numbered steps
- Work one step at a time
- After each step output CHECKPOINT BLOCK
- Wait for "committed" before next step
- End every response with 3-line RESUME BLOCK

Today's goal: [CHANGE THIS LINE ONLY]
```

## Resume Prompt (Save in Google Keep)

```
Read these files:
BRAIN: [raw link]
CHECKPOINT: [raw link]

Continue from next unfinished step only.
Do not repeat completed steps.
Output checkpoint block when done.
```

## End of Session Prompt (Save in Google Keep)

```
Session ending. Output:
1. Updated BRAIN.md (full content, under 300 words)
2. Updated CHECKPOINT.md
3. New RESULTS.csv rows if any
4. One line for DO_NOT_REPEAT.md if anything rejected
5. New FACTS.md entries if any
Keep short and ready to paste into GitHub.
```
