# AI Brain OS — Universal Project Template

> GitHub = Brain. AI = Worker. Notes App = Launcher.

This is your reusable operating system for any AI-assisted project.
Fork this once for every new project. Never build from scratch again.

---

## Quick Start (5 Steps)

1. Fork this repo → rename to your project (example: `three-slap-research`)
2. Fill in `SPEC.md` — what are you building?
3. Fill in `BRAIN.md` — what is the first task?
4. Update raw links in your Google Keep START note
5. Open any AI → paste START note → begin

---

## Full Repository Structure

```
ai-brain-os/
│
├── README.md                  ← You are here. Navigation map.
├── SPEC.md                    ← What are we building?
├── BRAIN.md                   ← Current reality (overwrite every session)
├── CHECKPOINT.md              ← Where work stopped (overwrite every step)
├── RESULTS.csv                ← Experiment results (append only)
├── FACTS.md                   ← Confirmed observations (append only)
├── DECISIONS.md               ← Why we chose something (append only)
├── DO_NOT_REPEAT.md           ← Rejected ideas (append only)
├── RED_TEAM.md                ← Why this might fail (overwrite weekly)
├── VALIDATION.md              ← Checklist before trusting results
├── WEEKLY_SUMMARY.md          ← Compressed knowledge (overwrite Sunday)
│
├── code/
│   ├── latest.py              ← Always newest code (overwrite)
│   └── YYYY-MM-DD-name.py    ← Dated archive (never delete)
│
├── prompts/
│   ├── startup.md             ← Paste at start of every session
│   ├── resume.md              ← Paste when switching accounts or models
│   ├── end-session.md         ← Paste before closing any chat
│   ├── red-team.md            ← Paste to attack your own work
│   ├── validate.md            ← Paste to check results
│   └── compress.md            ← Paste every Sunday
│
└── sessions/
    └── YYYY-MM-DD-session.md  ← One file per session (append only)
```

---

## File Rules — Replace or Add?

| File | Rule | Why |
|---|---|---|
| `BRAIN.md` | OVERWRITE every session | Always shows current reality |
| `CHECKPOINT.md` | OVERWRITE after every step | Always shows exact resume point |
| `code/latest.py` | OVERWRITE with newest code | Always runnable |
| `SPEC.md` | OVERWRITE only if project changes | Rarely changes |
| `RED_TEAM.md` | OVERWRITE weekly | Risks evolve over time |
| `WEEKLY_SUMMARY.md` | OVERWRITE every Sunday | Replaces old compression |
| `VALIDATION.md` | OVERWRITE only if checklist changes | Rarely changes |
| `RESULTS.csv` | APPEND new rows only | Preserve full experiment history |
| `FACTS.md` | APPEND new lines only | Facts never disappear |
| `DECISIONS.md` | APPEND new blocks only | Full decision audit trail |
| `DO_NOT_REPEAT.md` | APPEND new lines only | Grows as ideas get rejected |
| `sessions/` | ADD new dated file per session | Never overwrite old sessions |
| `code/` dated files | ADD new dated file per version | Never delete old code |

---

## AI Read Order (Paste This Into Any New AI)

When a new AI starts — whether Account B, Claude, ChatGPT, or Gemini — it reads files in this order:

```
1. SPEC.md         → What are we building?
2. BRAIN.md        → What is true right now?
3. CHECKPOINT.md   → Where did work stop?
4. RESULTS.csv     → What experiments ran?
5. DO_NOT_REPEAT.md → What must never be retried?
```

That is enough for any AI to resume work with zero re-explaining.

---

## Raw Links (Update After Forking)

Replace `ai-brain-os` with your forked repo name in all links below.

```
SPEC:        https://raw.githubusercontent.com/vishalm111296-commits/ai-brain-os/main/SPEC.md
BRAIN:       https://raw.githubusercontent.com/vishalm111296-commits/ai-brain-os/main/BRAIN.md
CHECKPOINT: https://raw.githubusercontent.com/vishalm111296-commits/ai-brain-os/main/CHECKPOINT.md
RESULTS:     https://raw.githubusercontent.com/vishalm111296-commits/ai-brain-os/main/RESULTS.csv
NO-REPEAT:   https://raw.githubusercontent.com/vishalm111296-commits/ai-brain-os/main/DO_NOT_REPEAT.md
VALIDATION:  https://raw.githubusercontent.com/vishalm111296-commits/ai-brain-os/main/VALIDATION.md
FACTS:       https://raw.githubusercontent.com/vishalm111296-commits/ai-brain-os/main/FACTS.md
RED_TEAM:    https://raw.githubusercontent.com/vishalm111296-commits/ai-brain-os/main/RED_TEAM.md
```

---

## Multi-AI Roles (Optional — Use After System Is Stable)

| AI | Role | When to Use |
|---|---|---|
| Claude | Builder — writes code and plans | Daily work |
| ChatGPT | Auditor — finds logical errors | After each experiment |
| Gemini | Critic — attacks assumptions | Before major decisions |
| Perplexity | Researcher — finds external evidence | When validating hypothesis |

Disagreement between AIs is more valuable than agreement.

---

## Forking for a New Project

1. Go to this repo on GitHub
2. Tap **Use this template** → **Create a new repository**
3. Name it your project (example: `three-slap-research`)
4. Fill `SPEC.md` and `BRAIN.md`
5. Update raw links in your phone notes
6. Start working

Same brain. New project. Zero setup time.
