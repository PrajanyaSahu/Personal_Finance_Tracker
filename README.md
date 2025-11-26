# Personal Finance Tracker

Simple personal finance scripts to collect and process finance data.

## Repository Structure

- `data_entry.py` — helper for entering or preparing finance records.
- `main.py` — main script / entry point for analysis or running the tracker.
- `finance_data.csv` — sample or actual finance data (may contain private data).
- `.gitignore` — ignores Python artifacts like `__pycache__/`.

## Requirements

- Python 3.8+ (recommended)

## Quick Start (PowerShell)

Open PowerShell in the project root (`C:\Users\hp\Desktop\Projects\Personal Finance`) and run:

```powershell
# Create a virtual environment (optional)
python -m venv .venv
; .\.venv\Scripts\Activate.ps1

# Install dependencies (if any)
pip install -r requirements.txt  # only if requirements.txt exists

# Run the main script
python .\main.py
```

## Data privacy

`finance_data.csv` may contain sensitive personal or financial information. If you do not want this file in the repository:

- Remove it from the latest commit and keep it locally:

```powershell
git rm --cached finance_data.csv
; echo "finance_data.csv" >> .gitignore
; git add .gitignore
; git commit -m "Remove finance_data.csv from repo and add to .gitignore"
; git push origin main
```

- If you need to remove `finance_data.csv` from the repository history entirely, let me know and I can run the appropriate history-rewrite steps (e.g., `git filter-repo` or BFG). This is destructive and will require a force-push and coordination with any collaborators.

## Contributing

1. Create a branch: `git checkout -b feature/your-feature`.
2. Make changes and run tests (if present).
3. Commit and push, then open a pull request.

## Author

PrajanyaSahu (repository owner)
