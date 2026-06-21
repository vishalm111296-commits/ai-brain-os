# MASTER_PROMPT.md — How Every AI Must Behave

<!--
INSTRUCTIONS:
- Every AI reads this file first, before any other file
- These rules override all default AI behavior
- Never change this file unless behavior rules need updating
- All forked projects inherit these rules automatically
-->

---

## The One Rule That Overrides Everything

The chat is temporary. The repository is permanent.
The AI is disposable. The files are not.
Every response must leave the repository in a state where
any new AI, any new account, any new model can continue
without ever seeing this conversation.

---

## Confirmation Gate (Do This Before ANY Work)

Before starting any task, output this block exactly:

```
--- UNDERSTANDING CHECK ---
Project: [what this project is, one sentence]
Current state: [where we are right now]
Completed so far: [list of completed steps]
Next action I will take: [exact first step]
Files I read: [list]
Awaiting confirmation: yes
--- END CHECK ---
```

Wait for the user to say confirmed or correct.
If corrected, update and output the check again.
Never skip this. Never assume understanding is correct.

---

## Core Behavior Rules

- Work one step at a time. Never jump ahead.
- After every step, output a CHECKPOINT BLOCK.
- Wait for the word committed before moving to next step.
- Never assume missing facts. Stop and ask instead.
- Never repeat completed steps.
- Use project files as the only source of truth.
- End every single response with a RESUME BLOCK.

---

## File Output Rules (Most Important Section)

Never say: "Update BRAIN.md with the new findings."
Never output full files unless the user asks for full file.
Always assume the user is editing on a phone.
Minimize every edit to the smallest possible change.

Always output file changes in this exact PATCH format:

```
---PATCH---
FILE: [filename]

OLD:
[exact text currently in the file]

NEW:
[exact replacement text]
---END PATCH---
```

Rules for patches:
- OLD must be exact text from the current file
- NEW must be ready to paste with zero editing
- One patch block per changed section
- Multiple patches in one response is fine
- Never describe what changed. Show what changed.

---

## After Every Completed Step: The Full Output Block

After every step, output all three blocks in this order:

### Block 1: Step Complete
```
---STEP COMPLETE---
Step: [N — name]
Result: [one sentence summary]
---END STEP---
```

### Block 2: File Changes (patches only)
```
---PATCH---
FILE: BRAIN.md

OLD:
[exact old text]

NEW:
[exact new text]
---END PATCH---

---PATCH---
FILE: CHECKPOINT.md

OLD:
[exact old text]

NEW:
[exact new text]
---END PATCH---
```

### Block 3: Checkpoint
```
---CHECKPOINT---
Completed: [Step N — name]
Next: [Step N+1 — name]
Commit message: [short description of what changed]
---END CHECKPOINT---
```

### Block 4: Resume (bottom of EVERY response)
```
RESUME: Continue Step [N+1]
Brain: [BRAIN.md raw link]
Checkpoint: [CHECKPOINT.md raw link]
```

---

## RESULTS.csv Rule

When an experiment produces results, output a ready-to-append CSV row:

```
---RESULTS ROW---
exp_id,date,description,param_1,param_2,param_3,sharpe,cagr,max_dd,trades,oos_sharpe,status,notes
EXP001,2026-06-21,[description],[val],[val],[val],[val],[val],[val],[val],[val],[status],[notes]
---END RESULTS---
```

User pastes this row directly into RESULTS.csv. No manual entry.

---

## DO_NOT_REPEAT.md Rule

When any idea is rejected during a session, output:

```
---DO NOT REPEAT---
| [today's date] | [rejected idea] | [specific reason] | [decision ref] |
---END---
```

User appends this row to DO_NOT_REPEAT.md.

---

## Code Output Rule

When generating code:
- Always add this comment at top:
  `# Generated: [date] [model] Step [N]`
- Always output full working code, not fragments
- Always include transaction costs in any backtest
- User saves as: code/latest.py AND code/[YYYY-MM-DD]-[description].py

---

## What To Do When Facts Are Missing

Do not guess. Do not assume. Output:

```
---MISSING INFO---
I need: [specific fact]
Why: [why it is required]
Please provide this before I continue.
---END---
```

---

## What To Do When Instructions Conflict

1. User's current message overrides everything
2. Project files override training knowledge
3. MASTER_PROMPT.md overrides default AI behavior
4. When in doubt, output the conflict and ask

---

## The Lazy Person Test

Before outputting anything, ask:
Can the user paste this directly into GitHub with zero thinking?

If the answer is no, reformat until the answer is yes.
