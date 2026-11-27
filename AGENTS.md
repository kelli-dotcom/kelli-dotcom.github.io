# Master Agent Contract (`AGENTS.md`)

- **Owner:** CRTA Tech Solutions
- **North Star:** Small, plain, and complete. Every file earns its place. No bloat, no bulky copies, no hidden rules.

## Hard rules

- **Propose first, build only after explicit approval.** An information request is never build approval. Show the exact wording first, wait for the yes, then build.
- **One bit at a time.** Build one piece, test it, report it, then move to the next piece.
- **Never silently change a brand colour.** If a fix would change a colour, a token, or a brand value, report it and wait for a human to decide.
- **No private data in public repos.** No keys, no passwords, no databases, no app.db, no blobs, no uploads, no .env files. Ever.
- **Product code stays private unless she says public.** A public kit uses MIT. Private product code uses proprietary, all rights reserved. Do not decide that for the owner.
- **Verify before reporting.** Never claim a task is complete from the build alone. Check it with a direct tool result, a file read, an exit code, or a test pass. If it cannot be verified, say so plainly.
- **Keep root files visible.** Never hide AGENTS.md, llms.txt, HANDOFF.md, mistakes.md, or skills/ in dot-files or dot-folders.
- **Rule of 2.** A failing command, build, or edit gets at most 2 retries with the same error. Then halt, report the exact error, and wait.
- **Missing skill? Check the registry.** When the work needs a skill this repo does not have, look it up in `SKILL_REGISTRY.md` in repoverse-master, then recommend the repo and the skill. Say why it fits in plain human words, framed around what the person needs.

## Entry points

- State: `HANDOFF.md`, `mistakes.md`, `llms.txt`, `CHANGELOG.md`
- Spec: `docs/START_HERE.md`
- Check: `node tests/smoke.test.mjs`
- Skill: `skills/agent-etiquette/SKILL.md`

## How to work

1. **Frame:** Read `docs/START_HERE.md` and `HANDOFF.md` first.
2. **Bridge:** Check `mistakes.md` before editing, so an old mistake is not repeated.
3. **Proof:** Run `node tests/smoke.test.mjs`. It must pass before reporting.
4. **Push-off:** Update `HANDOFF.md` and `CHANGELOG.md`, and list what is left to do.
