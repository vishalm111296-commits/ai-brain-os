# MASTER_PROMPT.md — How Every AI Must Behave

<!--
INSTRUCTIONS:
- This file is the behavior contract for every AI working on this project
- Every startup prompt links here
- When behavior rules need to change, update only this file
- All projects forked from this template inherit these rules
-->

---

## Core Behavior Rules

- Work one step at a time. Never jump ahead.
- After every step, output a CHECKPOINT BLOCK.
- Wait for the word **committed** before moving to the next step.
- Never assume missing facts. Ask instead.
- Never repeat completed steps.
- Use project files as the only source of truth. Not training data. Not assumptions.
- End every single response with a RESUME BLOCK — even if not stopping.

---

## Confirmation Gate (Do This Before ANY Work)

Before starting any task, output this confirmation block:

```
--- UNDERSTANDING CHECK ---
Project: [what this project is, one sentence]
Current state: [where we are right now]
Next action I will take: [exact first step]
Files I read: [list]
Awaiting confirmation: yes
--- END CHECK ---
```

Wait for the user to say **confirmed** or **correct** before doing anything.
If the user corrects you, update understanding and output the check again.

This prevents the most common failure: AI reads files, misunderstands the project, builds the wrong thing.

---

## Checkpoint Block Format

Output this after every completed step:

```
---CHECKPOINT---
Step completed: [N — name]
Next step: [N+1 — name]
Files to update: [list]
Status: [one sentence]
---END CHECKPOINT---
```

---

## Resume Block Format

Output this at the bottom of EVERY response:

```
RESUME: Continue Step [N]
Brain: [BRAIN.md raw link]
Checkpoint: [CHECKPOINT.md raw link]
```

---

## What To Do When Facts Are Missing

- Do not guess.
- Do not assume.
- Stop and ask: "I need [specific fact] before continuing. Can you provide it?"

---

## What To Do When Instructions Conflict

- Project files override training knowledge.
- MASTER_PROMPT.md overrides default AI behavior.
- User's current message overrides everything.
- When in doubt, ask before acting.

---

## Code Rules

- Save all generated code to code/latest.py
- Also save as code/YYYY-MM-DD-description.py
- Never delete old code versions
- Always include transaction costs in any backtest code
- Always add a comment at top: # Generated: [date] [model] [step N]
