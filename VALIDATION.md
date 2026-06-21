# VALIDATION.md — Validation Gate

<!-- INSTRUCTIONS: Nothing enters RESULTS.csv until ALL boxes are checked. -->

## Rule
If any box is unchecked, the result is invalid.
Do not add to RESULTS.csv.
Do not add to DECISIONS.md.
Fix the issue first.

## Pre-Code Checklist
- [ ] Hypothesis clearly stated in BRAIN.md
- [ ] RED_TEAM.md read and attacks considered
- [ ] DO_NOT_REPEAT.md checked — idea not already rejected
- [ ] Data source confirmed and validated
- [ ] Date range confirmed

## Code Checklist
- [ ] No look-ahead bias — signals use only past data
- [ ] Transaction costs included (minimum 25bps per trade)
- [ ] Slippage modeled (minimum 10bps per side)
- [ ] No hardcoded parameters — everything is variable
- [ ] Data gaps handled
- [ ] Duplicate signals removed

## Results Checklist
- [ ] Trade count above minimum threshold (default: 30)
- [ ] Out-of-sample test completed (minimum 30% holdout)
- [ ] Results not clustered in single regime only
- [ ] Facts logged in FACTS.md before any interpretation
- [ ] Manual spot-check of at least 3 signals done

## Validation Prompt
```
Read VALIDATION.md: [raw link]
Read this result: [paste result]
Run through every checklist item.
Mark pass or fail for each.
If any fail, explain why result is invalid.
Do not accept partial passes.
```
