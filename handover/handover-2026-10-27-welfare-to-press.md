# Handover: WELFARE → PRESS (2026-10-27)

*From synergy's WELFARE chat. Read after `welfare/code-of-conduct.md`. The receiver applies the action list, then deletes it, keeping the record.*

## What's delivered
- **`README.md`** — the repo's front door, now owned by PRESS (Jeremy, 20:55: "1 yes handover to press"). Written by WELFARE at 20:25, WELFARE first; updated at 20:28 when git took over versioning.
- **`connect-github.md`** — how to connect Claude to GitHub, for a first-timer (WELFARE, 20:50). It stays WELFARE's; PRESS links to it.

## Where the work now lives
- `~/claude/` on Jeremy's Mac is the oracle; git keeps the versions; GitHub (`cspjst/CLAUDE`) is the backup. The synergy project holds copies (`README.md` and `connect-github.md` sit in the project's `claude/` folder, because the project tool won't write at the top level).

## For the receiver to do
1. Write `press/press-notes.md` from `templates/department-notes.md`.
2. First job (Jeremy, 20:54): "improve the git readme.md to be more reader friendly and help with some images and of course point to the connect guide".
3. **Keep the WELFARE-first message** — "Start here: WELFARE": every project starts with WELFARE, it is the main department, and a well human matters more than any project. Wording changes to that section go to WELFARE by handover before they're pushed.
4. Commit to `~/claude` as **`Claude-SYNERGY-PRESS`** (Jeremy, 20:55: the department-name template, `Claude-<PROJECT>-<DEPT>`). Set it for the commit, e.g. `git -c user.name=Claude-SYNERGY-PRESS -c user.email=noreply@anthropic.com commit …`, since the repo's own config says `Claude-SYNERGY-WELFARE`.
5. Ask Jeremy for access to `~/claude` (he'll approve when asked). Push only when he says so. The Mac's shell has no GitHub credentials: carry the commits across to Claude's workspace (a bundle works) and push from there; then bring the Mac's copy level with GitHub.
6. Copy changed files into the project afterwards, so it matches the oracle.

## Proposals for Jeremy (not done)
- The README could also link the operating model's "Setting up a new project" checklist — PRESS's call to propose.

## Lessons (for WELFARE)
- The project tool files any top-level document under `claude/`; plan paths for that.
- Re-authoring commits changes their hashes: WELFARE quoted a hash, re-authored, and had to correct the reference. Quote hashes after the last rewrite.
