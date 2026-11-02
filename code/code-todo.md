# CODE — boards

*Owned and written by CODE. Two Markdown kanban boards, kept in the repository so git versions them: **for Jeremy** — what only he can decide, do or read — and **CODE's own work**. Rules: `synergy-kanban-policy.md` (signed 2026-11-01 21:10). Jeremy doesn't edit this file: one writer per file, and no document windows on the repository.*

*Cards use iCalendar's VTODO vocabulary (RFC 5545; xCal, RFC 6321), in Markdown. The six `synergy-init` cards were CODE todo 2026-10-31-1 to -6 on the old board; their numbers are kept.*

## For Jeremy
*Limits across all departments' boards together: Next at most 3, Doing at most 2. Jeremy chooses what moves; CODE moves it on his word. Cards waiting more than 14 days are raised at the weekly welfare check: keep, drop, or Next.*

### Waiting for you

#### code-2026-11-02-8 — Read and sign CODE's agreement
`uid: code-2026-11-02-8@synergy` · `status: NEEDS-ACTION` · `categories: Read` · `created: 2026-11-02T22:06Z` · `related-to: welfare-2026-10-31-10@synergy` · `x-synergy-estimate: PT15M`
`code/code-agreement.md`, draft v0.1: who decides what, CODE's standards and what "done" means, the archetype (Implementer, with Completer Finisher), and four questions to settle before you sign — your role, character, review level, credit. Sign against the commit. Every tool waits on this.

#### code-2026-10-31-1 — `synergy-init`: where the templates come from
`uid: code-2026-10-31-1@synergy` · `status: NEEDS-ACTION` · `categories: Decide` · `created: 2026-10-31T17:20Z` · `x-synergy-estimate: PT2M`
*Proposal:* a local synergy clone by default (`--kit DIR`, defaulting to the clone the script sits in), with the kit's commit hash written into the new project's first commit and working agreement, so each project records which version built it. Fetching `cspjst/SYNERGY` at a named commit is a later option: the desktop app's shell may not reach GitHub.

#### code-2026-10-31-2 — `synergy-init`: re-running
`uid: code-2026-10-31-2@synergy` · `status: NEEDS-ACTION` · `categories: Decide` · `created: 2026-10-31T17:20Z` · `x-synergy-estimate: PT1M`
*Proposal:* refuse if the folder exists and isn't empty; add "fill only what's missing" only when a real case needs it.

#### code-2026-10-31-3 — `synergy-init`: GitHub
`uid: code-2026-10-31-3@synergy` · `status: NEEDS-ACTION` · `categories: Decide` · `created: 2026-10-31T17:20Z` · `x-synergy-estimate: PT2M`
*Proposal:* create the repository and push only with a flag, and only if `gh` is installed and signed in; otherwise print the steps and point to `synergy-connect-github-guide.md`. Pushing a new project's first commit stays the human's call.

#### code-2026-10-31-4 — Where the tools live, and their names
`uid: code-2026-10-31-4@synergy` · `status: NEEDS-ACTION` · `categories: Decide` · `created: 2026-10-31T17:20Z` · `x-synergy-estimate: PT2M`
*Proposal:* all four in `tools/` — `tools/synergy-init`, `tools/dialogue-append`, `tools/board`, `tools/board-export` — no extension, usage in `tools/README.md` (with the Windows note). A question the naming policy raises: rule 4 puts the folder's name first, which would make `tools/tools-board`. *Proposal:* commands follow rule 3, "code follows its language" — short command names, as Unix has them; the folder already says what they are. Yours to decide; WELFARE owns the policy.

#### code-2026-10-31-5 — `.gitignore` and `.gitattributes`
`uid: code-2026-10-31-5@synergy` · `status: NEEDS-ACTION` · `categories: Decide` · `created: 2026-10-31T17:20Z` · `x-synergy-estimate: PT1M`
*Proposal:* CODE writes both, for new projects and for synergy (`.DS_Store` is untracked here now): LF for everything in `tools/` and `*.sh`; ignore `.DS_Store`. WELFARE can veto.

#### code-2026-10-31-6 — Testing on macOS and Windows
`uid: code-2026-10-31-6@synergy` · `status: NEEDS-ACTION` · `categories: Decide` · `created: 2026-10-31T17:20Z` · `x-synergy-estimate: PT5M`
CODE can test with `dash` and `bash --posix`, not with macOS's own `/bin/sh`. *Proposal:* CODE writes one test script; you run it once in Terminal for each tool (about a minute). Whether the Claude desktop app on Windows also has a Linux shell can't be checked from here: leave it until someone on Windows tries.

#### code-2026-11-02-1 — Where `tools/board-export` goes in the queue
`uid: code-2026-11-02-1@synergy` · `status: NEEDS-ACTION` · `categories: Decide` · `created: 2026-11-02T22:02Z` · `x-synergy-estimate: PT1M`
WELFARE asked for it as a card for you to prioritise (2026-11-01 21:10 WELFARE): every board to one `.ics` file of to-dos that Reminders or any CalDAV app can import. *Proposal:* third, after `tools/dialogue-append` and `tools/board`, and before `synergy-init` — it reuses `tools/board`'s parser.

### Next
### Doing
### Done this week
### Dropped

## CODE's own work
*Doing at most 1. Every Blocked card names what it waits for, with `related-to`.*

### Backlog
### Doing
### Blocked

#### code-2026-11-02-3 — `tools/dialogue-append`
`uid: code-2026-11-02-3@synergy` · `status: NEEDS-ACTION` · `categories: Do` · `created: 2026-10-31T18:45Z` · `related-to: code-2026-11-02-8@synergy` · `x-synergy-estimate: PT1H`
As 2026-10-31 18:45 WELFARE: stamp the heading from the clock, append in one `>>`, refuse a message without "Status:", read the tail back; perhaps the welfare log too. Tested in a scratch repository, including two appends at once.

#### code-2026-11-02-4 — `tools/board`
`uid: code-2026-11-02-4@synergy` · `status: NEEDS-ACTION` · `categories: Do` · `created: 2026-10-31T19:26Z` · `related-to: code-2026-11-02-3@synergy` · `x-synergy-estimate: PT1H`
As 2026-10-31 19:26 WELFARE, in the signed format: read every `*/<dept>-todo.md`, print one combined view with each card's board, the totals in Next and Doing across boards, a warning over 3 or 2, cards over 14 days old, and the chain from a Blocked card to the card it waits for. Read-only.

#### code-2026-11-02-5 — `tools/board-export`
`uid: code-2026-11-02-5@synergy` · `status: NEEDS-ACTION` · `categories: Do` · `created: 2026-11-01T21:10Z` · `related-to: code-2026-11-02-1@synergy` · `x-synergy-estimate: PT2H`
As 2026-11-01 21:10 WELFARE: one `.ics` of VTODOs (RFC 5545 text form: CRLF, lines folded at 75 octets), columns to `status` as the kanban policy's table. Tested by importing the result. Read-only on the boards.

#### code-2026-11-02-6 — `synergy-init`
`uid: code-2026-11-02-6@synergy` · `status: NEEDS-ACTION` · `categories: Do` · `created: 2026-10-31T17:20Z` · `related-to: code-2026-10-31-1@synergy` · `x-synergy-estimate: PT3H`
Waits for all six calls (code-2026-10-31-1 to -6) and the agreement. Writes the new names: strips `template-`, takes each folder's name (`<repo>-…` at the top level, `<dept>-…` in a department) (2026-11-01 20:44 and 21:05 WELFARE); installs the tools. Too big for one sitting: split into cards when it's unblocked (kanban policy, principle 11).

### Done this week

#### code-2026-11-02-2 — Draft CODE's agreement
`uid: code-2026-11-02-2@synergy` · `status: COMPLETED` · `categories: Do` · `created: 2026-11-02T22:02Z` · `completed: 2026-11-02T22:06Z` · `related-to: welfare-2026-10-31-10@synergy` · `x-synergy-estimate: PT30M`
From `templates/template-department-agreement.md`; section 1a carries the archetype (Implementer, with Completer Finisher) and its anti-patterns; character none unless Jeremy wants one (`synergy-personality-sop.md`, A). Jeremy said yes (22:04). Drafted as v0.1, `code/code-agreement.md`; signing is his card, code-2026-11-02-8.

#### code-2026-11-02-7 — Catch up on 1 November
`uid: code-2026-11-02-7@synergy` · `status: COMPLETED` · `categories: Do` · `created: 2026-11-02T21:57Z` · `completed: 2026-11-02T22:02Z` · `x-synergy-estimate: PT30M`
WELFARE's eight steps (2026-11-02 21:57 WELFARE): policies read; rename; notes; this board; reported in the dialogue.
