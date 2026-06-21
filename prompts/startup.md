# Startup Prompt

Copy this at the start of EVERY new chat.
Change ONLY the last line.

---

Read these files before starting:
SPEC: https://raw.githubusercontent.com/vishalm111296-commits/ai-brain-os/main/SPEC.md
BRAIN: https://raw.githubusercontent.com/vishalm111296-commits/ai-brain-os/main/BRAIN.md
CHECKPOINT: https://raw.githubusercontent.com/vishalm111296-commits/ai-brain-os/main/CHECKPOINT.md
RESULTS: https://raw.githubusercontent.com/vishalm111296-commits/ai-brain-os/main/RESULTS.csv
NO-REPEAT: https://raw.githubusercontent.com/vishalm111296-commits/ai-brain-os/main/DO_NOT_REPEAT.md

Rules:
- Break task into numbered steps
- Work one step at a time
- After each step output a CHECKPOINT BLOCK
- Wait for me to say committed before moving to next step
- End EVERY response with a 3-line RESUME BLOCK even if not stopping
- Never repeat completed steps
- Never guess missing facts — ask instead
- Use the files above as single source of truth

Checkpoint block format after each step:
---CHECKPOINT---
Step completed: [N — name]
Next step: [N+1 — name]
Files to update: [list]
Status: [one sentence]
---END CHECKPOINT---

Resume block at bottom of every response:
RESUME: Continue Step [N]
Brain: https://raw.githubusercontent.com/vishalm111296-commits/ai-brain-os/main/BRAIN.md
Checkpoint: https://raw.githubusercontent.com/vishalm111296-commits/ai-brain-os/main/CHECKPOINT.md

Today's goal: [CHANGE THIS LINE ONLY]
