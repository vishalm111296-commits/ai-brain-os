# VALIDATION.md — Validation Gate

<!--
INSTRUCTIONS FOR AI:
- Run through every item before adding anything to RESULTS.csv
- If any item fails, the result is invalid. Fix it first.
- Use the validation prompt below.
-->

---

## Validation Prompt

Paste this to validate any result:

```
Read VALIDATION.md: https://raw.githubusercontent.com/vishalm111296-commits/ai-brain-os/main/VALIDATION.md

Validate this result: [paste result here]

Run through every checklist item.
Mark each as PASS or FAIL.
If any item fails, explain why result is invalid.
Final verdict must be: VALID or INVALID.
No partial passes accepted.
```

---

## Pre-Code Checklist

- [ ] Hypothesis clearly stated in BRAIN.md
- [ ] RED_TEAM.md read and attacks considered
- [ ] DO_NOT_REPEAT.md checked — this idea is not already rejected
- [ ] Data source confirmed and validated
- [ ] Date range confirmed
- [ ] Universe defined and justified

---

## Code Checklist

- [ ] No look-ahead bias — signals use only past data
- [ ] Transaction costs included (minimum 25bps per trade)
- [ ] Slippage modeled (minimum 10bps per side)
- [ ] No hardcoded parameters — everything is a variable
- [ ] Data gaps handled and logged
- [ ] Duplicate signals removed
- [ ] Next-day execution only (no same-bar fills)

---

## Results Checklist

- [ ] Trade count above minimum (default: 30 trades)
- [ ] Out-of-sample test completed (minimum 30% holdout)
- [ ] Results tested across multiple market regimes
- [ ] Facts logged in FACTS.md before any interpretation
- [ ] Manual spot-check of at least 3 individual signals done
- [ ] Walk-forward validation completed
