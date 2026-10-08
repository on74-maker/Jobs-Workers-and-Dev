# CLAUDE.md

## Project
- Course research project on jobs, workers, and development.
- Data: CPS ASEC (Current Population Survey, Annual Social and Economic Supplement) from IPUMS.
- Analysis lives in a Python notebook (`.ipynb`) and runs in Google Colab.

## Code style
- Keep code simple: basic pandas, numpy, and matplotlib; no clever tricks.
- Put a short comment on every line of code, saying what it does.
- Use clear variable names (e.g., `df_asec`, `wage_by_year`).
- Prefer small cells that each do one thing.

## Colab notes
- Code must run top to bottom in a fresh Colab session.
- Install or import everything in the first cell.
- Load data from a path or Google Drive mount that is stated in a comment.
- Do not commit raw IPUMS data files (large and covered by IPUMS terms of use); keep them out of git (`.gitignore`).

## Communication
- Explain every change in plain English: what changed and why, with no jargon.
- Say what a result means, not just what the code printed.

## Git workflow
- Develop on the assigned branch, commit with clear messages, and push.
- When done, merge the branch into `main` and push `main`.
- Do NOT open pull requests.
