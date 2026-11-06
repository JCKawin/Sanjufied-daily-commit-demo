# Daily 4AM Commit Workflow Demo

This repository demonstrates a GitHub Action that:

1. Runs every day at **4:00 AM IST** (Asia/Kolkata)
2. Checks the current contents of the repository
3. Updates `daily-log.txt` with a timestamp and file list
4. Commits and pushes the change

## Workflow file

See `.github/workflows/daily-commit.yml`

### Notes
- Schedule uses the official timezone support (available since March 2026).
- GitHub Actions schedules are best-effort and may be delayed a few minutes under high load.
- Requires `contents: write` permission (already set in the workflow).
- You can also trigger it manually from the Actions tab.

To use this in another repository, copy the workflow file into `.github/workflows/`.
