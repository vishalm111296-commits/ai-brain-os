# Code Folder

All AI-generated code lives here.

## Rules
- Never delete old versions
- Always use dated filenames
- Latest working version is always named `latest.py`

## File Naming
```
code/
├── latest.py              ← Always the current working version
├── backtest_2026-06-21.py ← Dated archive versions
├── backtest_2026-06-22.py
├── optimize_2026-06-23.py
└── scanner_2026-06-24.py
```

## Rule
Every time AI generates new code:
1. Save as dated file  (example: backtest_2026-06-21.py)
2. Also overwrite latest.py with same content
3. Commit both

That way you always have the latest AND full history.
