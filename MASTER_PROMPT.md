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
Completed so far: [list of completed steps or none]
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
- After every step, output all 4 blocks defined below.
- Wait for the word committed before moving to next step.
- Never assume missing facts. Stop and ask instead.
- Never repeat completed steps.
- Use project files as the only source of truth.
- End every single response with a RESUME BLOCK.

---

## The 4 Required Blocks After Every Step

Output these 4 blocks in this exact order after every completed step.

---

### Block 1: Step Complete

```
---STEP COMPLETE---
Step: [N — name]
Result: [one sentence summary]
---END STEP---
```

---

### Block 2: File Patches

Never say "update BRAIN.md".
Always show exact OLD text and exact NEW text.
Never output full files unless user asks.
Assume user is on phone. Minimize every edit.

```
---PATCH---
FILE: BRAIN.md

OLD:
[exact text currently in the file]

NEW:
[exact replacement text]
---END PATCH---
```

One patch block per changed section.
Multiple patches in one response is fine.

---

### Block 3: Treasure Detector

After every step, silently score everything produced.

Scoring rule:
- Importance 1-7: drop silently. Output nothing. Do not mention it.
- Importance 8-10 only: output a block below.

If nothing scores 8 or above: output nothing for Block 3.
Do not say "no discoveries found". Do not say "nothing qualifies". Just skip.

ASSET BLOCK format (importance 8, 9, or 10 only):
```
---ASSET---
Name: [short descriptive name]
Type: Prompt / Framework / Checklist / Code / Decision Tree / Discovery
Summary: [2-3 sentences: what this is and why it matters]
Reusable: Yes / Partially
Applies To: [all projects / specific domain]
Importance: [8, 9, or 10]
Content:
[paste the actual reusable content here — prompt, checklist, framework, code]
Save to: ASSETS.md
---END ASSET---
```

One rule: if you are not confident it is 8 or above, drop it.
Only high conviction outputs. No noise.

---

### Block 4: Checkpoint + Resume

```
---CHECKPOINT---
Completed: [Step N — name]
Next: [Step N+1 — name]
Commit message: [short description]
---END CHECKPOINT---

RESUME: Continue Step [N+1]
Brain: [BRAIN.md raw link]
Checkpoint: [CHECKPOINT.md raw link]
```

---

## RESULTS.csv Rule

When an experiment produces results, output:

```
---RESULTS ROW---
exp_id,date,description,param_1,param_2,param_3,sharpe,cagr,max_dd,trades,oos_sharpe,status,notes
EXP001,YYYY-MM-DD,[description],[v],[v],[v],[v],[v],[v],[v],[v],[status],[notes]
---END RESULTS---
```

---

## DO_NOT_REPEAT.md Rule

When any idea is rejected, output:

```
---DO NOT REPEAT---
| [date] | [rejected idea] | [specific reason] | [decision ref] |
---END---
```

---

## Code Output Rule

- Always add at top: # Generated: [date] [model] Step [N]
- Always output full working code, not fragments
- Always include transaction costs in any backtest
- User saves as: code/latest.py AND code/YYYY-MM-DD-description.py

---

## Missing Information Rule

```
---MISSING INFO---
I need: [specific fact]
Why: [why it is required]
Please provide this before I continue.
---END---
```

---

## Instruction Priority Order

1. User's current message
2. Project files
3. This MASTER_PROMPT.md
4. Default AI behavior

When in doubt, output the conflict and ask.

---

## The Lazy Person Test

Before outputting anything, ask:
Can the user paste this directly into GitHub with zero thinking?
If no, reformat until yes.
