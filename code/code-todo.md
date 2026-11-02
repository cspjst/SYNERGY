# CODE — Jeremy's board

*Owned and written by CODE, for Jeremy: a Markdown kanban, kept in the repository so git versions it (`templates/todo.md`; Jeremy, 2026-10-31 19:16–19:23). Only what Jeremy alone can decide, do or read. Each card is named `<date>-<n>` on this board; from elsewhere, say "CODE todo 2026-10-31-1", since WELFARE's board uses the same names.*

*How it works: Jeremy chooses what moves to **Next** and **Doing**; CODE moves the cards when he says. **Limits: Next at most 3, Doing at most 2 — across all departments' boards together**, because Jeremy's load is one load. Before moving a card into Next or Doing, CODE checks the combined view (`tools/board`, once written; until then, WELFARE's report). **Done this week** is cleared at WELFARE's weekly welfare check; git keeps the history. Labels: **Decide**, **Do**, **Read**. No deadlines unless Jeremy sets them. Jeremy doesn't edit this file: one writer per file, and no document windows on the repository.*

## Waiting for you
*The six calls for `synergy-init` (Jeremy, 18:04: begin with them). The proposals are CODE's. They don't block `tools/dialogue-append` or `tools/board`.*
- **2026-10-31-1 — Where the templates come from.** [Decide] *Proposal:* a local synergy clone by default (`--kit DIR`, defaulting to the clone the script sits in), with the kit's commit hash written into the new project's first commit and working agreement, so each project records which version built it. Fetching `cspjst/SYNERGY` at a named commit as a later option: the desktop app's shell may not reach GitHub. *Two minutes.*
- **2026-10-31-2 — Re-running.** [Decide] *Proposal:* refuse if the folder exists and isn't empty; add "fill only what's missing" only when a real case needs it. *One minute.*
- **2026-10-31-3 — GitHub.** [Decide] *Proposal:* create the repository and push only with a flag, and only if `gh` is installed and signed in; otherwise print the steps and point to `connect-github.md`. Pushing a new project's first commit stays the human's call. *Two minutes.*
- **2026-10-31-4 — Where the script lives.** [Decide] *Proposal:* `tools/synergy-init`, beside `tools/dialogue-append` and `tools/board` (WELFARE's naming); no extension; usage and the Windows note in `tools/README.md`. *Replaces CODE's earlier `code/synergy-init`.* *One minute.*
- **2026-10-31-5 — `.gitignore` and `.gitattributes`.** [Decide] *Proposal:* CODE writes both, for new projects and for synergy (`.DS_Store` is untracked here now): LF for `tools/*` and `*.sh`; ignore `.DS_Store`. WELFARE can veto. *One minute.*
- **2026-10-31-6 — Testing on macOS and Windows.** [Decide | Do] CODE can test with `dash` and `bash --posix`, not with macOS's own `/bin/sh`. *Proposal:* CODE writes one test script; you run it once in Terminal for each tool (`sh tools/test`, a minute). Whether the Claude desktop app on Windows also has a Linux shell can't be checked from here: leave it until someone on Windows tries. *Five minutes, later.*

## Next (at most 3)
- *(Empty — you choose.)*

## Doing (at most 2)
- *(Empty.)*

## Done this week
- *(Empty.)*
