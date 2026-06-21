# AI Brain OS — Universal Project Template

> GitHub = Brain. AI = Worker. Notes App = Launcher.

Fork this once for every new project. Never build from scratch again.

---

## Quick Start (5 Steps)

1. Fork this repo → rename to your project (example: `three-slap-research`)
2. Fill `PROJECT_BRIEF.md` — what are you building and why?
3. Fill `BRAIN.md` — what is the current state and first task?
4. Replace `ai-brain-os` with your new repo name in your phone START note
5. Open any AI → paste START note → begin

---

## File Structure

```
ai-brain-os/
│
├── PROJECT_BRIEF.md        ← Read FIRST. What, why, success, failure.
├── MASTER_PROMPT.md        ← AI behavior contract. Inherited by all projects.
├── SPEC.md                 ← Technical rules and constraints.
├── BRAIN.md                ← Current reality. Overwrite every session.
├── CHECKPOINT.md           ← Where work stopped. Overwrite every step.
├── RESULTS.csv             ← Experiment results. Append only.
├── FACTS.md                ← Confirmed observations. Append only.
├── DECISIONS.md            ← Why we chose something. Append only.
├── DO_NOT_REPEAT.md        ← Rejected ideas. Append only.
├── RED_TEAM.md             ← Why this might fail. Overwrite weekly.
├── VALIDATION.md           ← Checklist before trusting results.
├── WEEKLY_SUMMARY.md       ← Compressed memory. Overwrite Sundays.
│
├── code/
│   ├── latest.py           ← Always newest code. Overwrite.
│   └── YYYY-MM-DD-name.py  ← Dated archive. Never delete.
│
├── prompts/
│   ├── startup.md          ← Paste at start of every session.
│   ├── resume.md           ← Paste when switching accounts or models.
│   ├── end-session.md      ← Paste before closing any chat.
│   ├── red-team.md         ← Paste to attack your own work.
│   ├── validate.md         ← Paste to check results.
│   └── compress.md         ← Paste every Sunday.
│
└── sessions/               ← Archive only. One dated file per session.
```

---

## Core Files vs Advanced Files

This is the most important distinction in the system.

### Core Files — Update These Every Session

These 4 files are the minimum viable brain.
If you only ever update these, the system still works.

| File | When | Rule |
|---|---|---|
| `PROJECT_BRIEF.md` | Once at start | Overwrite only if purpose changes |
| `BRAIN.md` | Every session end | Overwrite |
| `CHECKPOINT.md` | After every step | Overwrite |
| `RESULTS.csv` | After every experiment | Append new row |

### Advanced Files — Update When Relevant

These files add depth over time but will not break the system if skipped.

| File | When | Rule |
|---|---|---|
| `SPEC.md` | Setup + major changes | Overwrite |
| `DO_NOT_REPEAT.md` | After any rejection | Append one line |
| `RED_TEAM.md` | Every Sunday | Overwrite |
| `VALIDATION.md` | Before trusting results | Run checklist |
| `FACTS.md` | After confirmed observations | Append |
| `DECISIONS.md` | After major choices | Append |
| `WEEKLY_SUMMARY.md` | Every Sunday | Overwrite |
| `MASTER_PROMPT.md` | Once — rarely changes | Overwrite only if behavior rules change |

---

## AI Read Order

Minimum read (paste this into any new AI):

```
1. PROJECT_BRIEF.md  → What is this project?
2. BRAIN.md          → What is true right now?
3. CHECKPOINT.md     → Where did work stop?
```

Full read (for new experiments or major sessions):

```
1. PROJECT_BRIEF.md
2. BRAIN.md
3. CHECKPOINT.md
4. RESULTS.csv
5. DO_NOT_REPEAT.md
```

Full read is 5 files. Minimum read is 3 files. Never more than 5 at startup.

---

## Raw Links (Replace repo name after forking)

```
BRIEF:       https://raw.githubusercontent.com/vishalm111296-commits/ai-brain-os/main/PROJECT_BRIEF.md
MASTER:      https://raw.githubusercontent.com/vishalm111296-commits/ai-brain-os/main/MASTER_PROMPT.md
BRAIN:       https://raw.githubusercontent.com/vishalm111296-commits/ai-brain-os/main/BRAIN.md
CHECKPOINT: https://raw.githubusercontent.com/vishalm111296-commits/ai-brain-os/main/CHECKPOINT.md
RESULTS:     https://raw.githubusercontent.com/vishalm111296-commits/ai-brain-os/main/RESULTS.csv
NO-REPEAT:   https://raw.githubusercontent.com/vishalm111296-commits/ai-brain-os/main/DO_NOT_REPEAT.md
VALIDATION:  https://raw.githubusercontent.com/vishalm111296-commits/ai-brain-os/main/VALIDATION.md
FACTS:       https://raw.githubusercontent.com/vishalm111296-commits/ai-brain-os/main/FACTS.md
RED_TEAM:    https://raw.githubusercontent.com/vishalm111296-commits/ai-brain-os/main/RED_TEAM.md
SPEC:        https://raw.githubusercontent.com/vishalm111296-commits/ai-brain-os/main/SPEC.md
```

---

## Multi-AI Roles

| AI | Role | When |
|---|---|---|
| Claude | Builder — writes code and plans | Daily work |
| ChatGPT | Auditor — finds logical errors | After each experiment |
| Gemini | Critic — attacks assumptions | Before major decisions |
| Perplexity | Researcher — finds external evidence | When validating hypothesis |

Disagreement between AIs is more valuable than agreement.

---

## Maintenance Fatigue Test

Before adding any new file, ask:

> Will I still update this from my phone at 1am after the AI has hit its token limit three times?

If the answer is no, merge it into BRAIN.md or remove it from the daily workflow.

---

## When Tokens Run Out Mid-Task

1. Every AI response already ends with a RESUME BLOCK
2. Copy the resume block from the last complete response
3. Open new account or model
4. Paste resume.md prompt with the raw links
5. New AI reads PROJECT_BRIEF + BRAIN + CHECKPOINT and continues
6. Zero work lost

---

## Forking for a New Project

1. Go to this repo → tap **Use this template** → **Create a new repository**
2. Name it your project
3. Fill `PROJECT_BRIEF.md` and `BRAIN.md`
4. In all your phone notes: replace `ai-brain-os` with new repo name
5. Start working

Same brain. New project. 5 minutes setup.
