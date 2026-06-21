# RED_TEAM.md — Why This Project Might Fail

<!--
INSTRUCTIONS FOR AI:
- OVERWRITE this file weekly
- Read this before every major decision
- Use the red team prompt below to force critic mode
-->

---

## Red Team Prompt

Paste this to make any AI attack your work:

```
Read RED_TEAM.md: https://raw.githubusercontent.com/vishalm111296-commits/ai-brain-os/main/RED_TEAM.md
Read RESULTS.csv: https://raw.githubusercontent.com/vishalm111296-commits/ai-brain-os/main/RESULTS.csv
Read FACTS.md: https://raw.githubusercontent.com/vishalm111296-commits/ai-brain-os/main/FACTS.md

Attack the current best result.
Find every reason it could be wrong or misleading.
Do not suggest improvements. Only find problems.
Output as numbered list. Label each: High / Medium / Low severity.
```

---

## Standard Attacks (Check Every Project Against These)

- Survivorship bias: are failed or delisted assets missing from the data?
- Look-ahead bias: do any signals use future data even accidentally?
- Selection bias: was the test universe chosen after seeing results?
- Regime dependency: does it only work in one type of market?
- Overfitting: too many parameters tested on too little data?
- Transaction costs: are realistic costs actually included in the code?
- Sample size: are there enough events to draw valid conclusions?
- Data quality: are there gaps, errors, or wrong adjustments in data?
- Implementation gap: will live trading differ from backtest assumptions?

---

## Project-Specific Failure Modes

ATTACK-001:
Risk: [describe failure mode]
Severity: High / Medium / Low
Mitigation: [how to check or fix this]
Status: Open / Mitigated
