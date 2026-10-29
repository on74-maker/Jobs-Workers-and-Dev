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

## Weights and charts
- Use `asecwt` for person-level survey weights. Use it in every table and chart.
- Before any chart, print the weighted table it will show, with labels and 1 decimal.
- A chart shows exactly the printed table, and axis labels give units.
- All y-axis scales and labels should include 0.

## Communication
- Explain every change in plain English: what changed and why, with no jargon.
- Say what a result means, not just what the code printed.
- Never write narrative text, interpretation, or write-ups on your own. Only insert text I give you, exactly as written.

## Lessons
@LESSONS.md
- When I correct you or state a preference, add a line to LESSONS.md: what happened and the rule for next time.
- When I paste an error from Colab, or you find a mistake in your code, fix it and add a line on the cause.
- Update an existing line instead of repeating it. Keep each line short.
- Commit LESSONS.md with your other changes.

## Git workflow
- Always sync to `main` first (fetch and merge `origin/main` into your branch) so you have the latest files in the repo.
- Develop on the assigned branch, commit with clear messages, and push.
- When done, merge the branch into `main` and push `main`.
- Do NOT open pull requests.
