# RED_TEAM.md — Why This Project Might Fail

<!-- INSTRUCTIONS: OVERWRITE weekly. Add new attacks as they are discovered. -->
<!-- Use this file before every major decision. Ask AI to attack using this file. -->

## Purpose
This file stores every known way this project could be wrong.
Read it before major decisions.
Use it to prompt AI into critic mode:
"Attack this project using RED_TEAM.md. Find every reason the current result could be invalid."

## Red Team Prompt
```
Read RED_TEAM.md: [raw link]
Read RESULTS.csv: [raw link]
Read FACTS.md: [raw link]

Attack the current best result.
Find every reason it could be wrong or misleading.
Do not suggest improvements. Only find problems.
Output as numbered list of attacks.
```

## Known Failure Modes

ATTACK-001: [date]
Risk: [describe the failure mode]
Severity: High / Medium / Low
Mitigation: [how to check for this]
Status: Open / Mitigated

---

## Standard Attacks (Check These For Every Project)

- Survivorship bias: are failed/delisted assets missing from data?
- Look-ahead bias: do signals use any future data?
- Selection bias: was the universe chosen after seeing results?
- Regime dependency: does it only work in one market condition?
- Overfitting: too many parameters tested on too little data?
- Transaction costs: are realistic costs included?
- Sample size: are there enough events to be statistically valid?
- Data quality: are there gaps, errors, or adjustments in the data?
