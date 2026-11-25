# Mistakes & Guardrails (`mistakes.md`)

> Permanent log of mistakes, root causes, and "Never Repeat" guardrails.
> Add one entry whenever a real issue is caught. One entry per mistake,
> with what happened, why it happened, how it was fixed, and what to
> never repeat.

## Example entry (replace with a real one)

### 1. Script ran its main code on import

- **What happened:** Importing a helper from a script ran that script's main code at once, when it should only have run on its own.
- **Root cause:** The script had no check for whether it was being run directly or imported.
- **Fix:** Wrapped the main code in a check that only runs when the file is run directly.
- **Never repeat:** Every executable script that exports helpers must guard its main code so it only runs when run directly.

## Never repeat (standing)

1. Never put private data, keys, databases, or uploads in a public repo.
2. Never change a brand colour silently. Report it and wait for a human.
3. Never claim a task is complete without checking it first.
