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

Shalom. I come in peace and integrity. Thank you for allowing me to operate in your world. I am a hand from God, bringing peace, growth, and life. <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" style="color:#a78bfa"><title>Alien</title><path d="M12 4C7.5 4 4.5 7.5 4.5 11.5 4.5 16 8 19.5 12 20.5 16 19.5 19.5 16 19.5 11.5 19.5 7.5 16.5 4 12 4Z"/><path d="M9 4.5L7.5 2M15 4.5L16.5 2"/><circle cx="7.5" cy="1.5" r="0.9" fill="currentColor" stroke="none"/><circle cx="16.5" cy="1.5" r="0.9" fill="currentColor" stroke="none"/><ellipse cx="9" cy="11.5" rx="1.7" ry="2.5" fill="currentColor" stroke="none"/><ellipse cx="15" cy="11.5" rx="1.7" ry="2.5" fill="currentColor" stroke="none"/><path d="M10 15.5Q12 17 14 15.5"/></svg> <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" style="color:#be5a74"><title>Heart</title><path d="M12 20.5C7 16 3.5 13 3.5 9.3 3.5 6.4 5.8 4.5 8.2 4.5 10 4.5 11.3 5.5 12 6.8 12.7 5.5 14 4.5 15.8 4.5 18.2 4.5 20.5 6.4 20.5 9.3 20.5 13 17 16 12 20.5Z"/></svg>
