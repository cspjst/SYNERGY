# CODE — boards

*Owned and written by CODE. Two Markdown kanban boards, kept in the repository so git versions them: **for Jeremy** — what only he can decide, do or read — and **CODE's own work**. Rules: `synergy-kanban-policy.md` (signed 2026-11-01 21:10). Jeremy doesn't edit this file: one writer per file, and no document windows on the repository.*

*Cards use iCalendar's VTODO vocabulary (RFC 5545; xCal, RFC 6321), in Markdown. The six `synergy-init` cards were CODE todo 2026-10-31-1 to -6 on the old board; their numbers are kept.*

## For Jeremy
*Limits across all departments' boards together: Next at most 3, Doing at most 2. Jeremy chooses what moves; CODE moves it on his word. Cards waiting more than 14 days are raised at the weekly welfare check: keep, drop, or Next.*

### Waiting for you

#### code-2026-11-02-17 — CODE's agreement v0.3: accessibility in the standards
`uid: code-2026-11-02-17@synergy` · `status: NEEDS-ACTION` · `categories: Decide` · `created: 2026-11-02T22:42Z` · `x-synergy-estimate: PT5M`
Jeremy (22:37): "firstly - WCAG - well done". *Proposal:* section 3 gains a line — any tool that makes a page meets WCAG 2.2 level AA where it applies: colour never the only signal (1.4.1), text contrast 4.5:1 (1.4.3), usable at 200% zoom (1.4.4). CODE drafts v0.3; you sign it.

#### code-2026-11-02-1 — Where `tools/board-export` goes in the queue
`uid: code-2026-11-02-1@synergy` · `status: NEEDS-ACTION` · `categories: Decide` · `created: 2026-11-02T22:02Z` · `x-synergy-estimate: PT1M`
WELFARE asked for it as a card for you to prioritise (2026-11-01 21:10 WELFARE): every board to one `.ics` file of to-dos that Reminders or any CalDAV app can import. *Proposal:* third, after `tools/board` and `tools/dialogue-append` (the order since 22:17), and before `synergy-init` — it reuses `tools/board`'s reading of the cards.

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

### Next
### Doing
### Done this week

#### code-2026-11-02-9 — `tools/board`: its interface
`uid: code-2026-11-02-9@synergy` · `status: COMPLETED` · `categories: Decide` · `created: 2026-11-02T22:18Z` · `completed: 2026-11-02T22:21Z` · `x-synergy-estimate: PT3M`
**Decided** (Jeremy, 22:20: "yes to 1,2,3,4 lets see what you come up with :)"). CODE's proposals, KISS:
1. **Run:** `tools/board` from anywhere in the repository; no options in version 1. It finds the repository's top, reads `<dept>/<dept>-todo.md` for every department (not `templates/`), writes the page and prints its path. It doesn't open the browser itself: `open synergy-board.html` is one more word, and Mac-only.
2. **The page:** `synergy-board.html` at the top level — named by the naming policy (repository first), rebuilt every run. Kept out of git: one line in `.gitignore`, which is your card code-2026-10-31-5; until you answer that, in `.git/info/exclude`, which only this Mac sees.
3. **The text view:** dropped for version 1 (KISS); back as `--text` if anyone misses it.
4. **The look:** plain HTML and CSS, light and dark following the Mac, no colour but red for over-limit; each card as it is in the Markdown, one block per card.
Card code-2026-10-31-4 (where the tools live, rule 3 or rule 4 of the naming policy) also decides this tool's name; `tools/board` is assumed here.

#### code-2026-11-02-8 — Read and sign CODE's agreement
`uid: code-2026-11-02-8@synergy` · `status: COMPLETED` · `categories: Read` · `created: 2026-11-02T22:06Z` · `completed: 2026-11-02T22:12Z` · `related-to: welfare-2026-10-31-10@synergy` · `x-synergy-estimate: PT15M`
`code/code-agreement.md`, draft v0.1: who decides what, CODE's standards and what "done" means, the archetype (Implementer, with Completer Finisher), and four questions to settle before you sign — your role, character, review level, credit. Signed by Jeremy 2026-11-02 22:12, against `a24b5c9` ("agreement is good i sign it off pls").

### Dropped

## CODE's own work
*Doing at most 1. Every Blocked card names what it waits for, with `related-to`.*

### Backlog

#### code-2026-11-02-3 — `tools/dialogue-append`
`uid: code-2026-11-02-3@synergy` · `status: NEEDS-ACTION` · `categories: Do` · `created: 2026-10-31T18:45Z` · `x-synergy-estimate: PT1H`
As 2026-10-31 18:45 WELFARE: stamp the heading from the clock, append in one `>>`, refuse a message without "Status:", read the tail back; perhaps the welfare log too. Tested in a scratch repository, including two appends at once. Second, after `tools/board` (Jeremy, 22:17).


#### code-2026-11-02-10 — `tools/board` v2: your board first, in colour
`uid: code-2026-11-02-10@synergy` · `status: NEEDS-ACTION` · `categories: Do` · `created: 2026-11-02T22:42Z` · `related-to: code-2026-11-02-4@synergy` · `x-synergy-estimate: PT2H`
Jeremy's v2 (Jeremy, 22:42, on CODE's ideas of 22:38): "card for v2 6, 1, 2, and 8". **(6)** one board at the top for Jeremy: every department's Waiting for you, Next and Doing merged ("concur"); **(1)** Decide, Do and Read as coloured, labelled pills; **(2)** a department accent stripe on each card and section; **(8)** shorter card numbers inside a department's own section. Colour never alone — a word or shape with it (WCAG 2.2, 1.4.1); text contrast 4.5:1 or more in light and dark (1.4.3), checked with a contrast tool, not by eye.

#### code-2026-11-02-11 — `tools/board`: WELFARE first
`uid: code-2026-11-02-11@synergy` · `status: NEEDS-ACTION` · `categories: Do` · `created: 2026-11-02T22:42Z` · `related-to: code-2026-11-02-4@synergy` · `x-synergy-estimate: PT10M`
Idea 7, "yes" (Jeremy, 22:42, on CODE's ideas of 22:38), but in neither version list — a card of its own; it can ride with v2 if Jeremy says. WELFARE, the main department, leads the page.

#### code-2026-11-02-12 — `tools/board` v3: column state
`uid: code-2026-11-02-12@synergy` · `status: NEEDS-ACTION` · `categories: Do` · `created: 2026-11-02T22:42Z` · `related-to: code-2026-11-02-10@synergy` · `x-synergy-estimate: PT30M`
Idea 3, "yes" (Jeremy, 22:42, on CODE's ideas of 22:38); v3, one at a time. Doing tinted as live; Done faded; Dropped struck through.

#### code-2026-11-02-13 — `tools/board` v3: limit gauges
`uid: code-2026-11-02-13@synergy` · `status: NEEDS-ACTION` · `categories: Do` · `created: 2026-11-02T22:42Z` · `related-to: code-2026-11-02-10@synergy` · `x-synergy-estimate: PT30M`
Idea 4, "yes nice idea" (Jeremy, 22:42, on CODE's ideas of 22:38); v3, one at a time. Next and Doing totals as pills: green under the limit, amber at it, red over — each with its number, so colour isn't the only signal.

#### code-2026-11-02-14 — `tools/board` v3: card age
`uid: code-2026-11-02-14@synergy` · `status: NEEDS-ACTION` · `categories: Do` · `created: 2026-11-02T22:42Z` · `related-to: code-2026-11-02-10@synergy` · `x-synergy-estimate: PT1H`
Idea 5, "new card save for later" (Jeremy, 22:42, on CODE's ideas of 22:38); v3, one at a time. Borders warm to amber at 14 days — the kanban policy's garbage collector (principle 6) — from each card's `created`, with the age written on the card.

#### code-2026-11-02-15 — `tools/board` v3: click to expand
`uid: code-2026-11-02-15@synergy` · `status: NEEDS-ACTION` · `categories: Do` · `created: 2026-11-02T22:42Z` · `related-to: code-2026-11-02-10@synergy` · `x-synergy-estimate: PT30M`
Idea 9, "yes" (Jeremy, 22:42, on CODE's ideas of 22:38); v3, one at a time. Each card opens to its description with HTML's `<details>`: no script.

#### code-2026-11-02-16 — `tools/board` v3: "waits for" links
`uid: code-2026-11-02-16@synergy` · `status: NEEDS-ACTION` · `categories: Do` · `created: 2026-11-02T22:42Z` · `related-to: code-2026-11-02-10@synergy` · `x-synergy-estimate: PT1H`
Idea 10, "also v good" (Jeremy, 22:42, on CODE's ideas of 22:38); v3, one at a time. A Blocked card shows what it waits for (`related-to`), and a click jumps to that card, across boards.

### Doing

### Blocked

#### code-2026-11-02-5 — `tools/board-export`
`uid: code-2026-11-02-5@synergy` · `status: NEEDS-ACTION` · `categories: Do` · `created: 2026-11-01T21:10Z` · `related-to: code-2026-11-02-1@synergy` · `x-synergy-estimate: PT2H`
As 2026-11-01 21:10 WELFARE: one `.ics` of VTODOs (RFC 5545 text form: CRLF, lines folded at 75 octets), columns to `status` as the kanban policy's table. Tested by importing the result. Read-only on the boards.

#### code-2026-11-02-6 — `synergy-init`
`uid: code-2026-11-02-6@synergy` · `status: NEEDS-ACTION` · `categories: Do` · `created: 2026-10-31T17:20Z` · `related-to: code-2026-10-31-1@synergy` · `x-synergy-estimate: PT3H`
Waits for all six calls (code-2026-10-31-1 to -6) and the agreement. Writes the new names: strips `template-`, takes each folder's name (`<repo>-…` at the top level, `<dept>-…` in a department) (2026-11-01 20:44 and 21:05 WELFARE); installs the tools. Too big for one sitting: split into cards when it's unblocked (kanban policy, principle 11).

### Done this week

#### code-2026-11-02-4 — `tools/board`: the boards in a browser
`uid: code-2026-11-02-4@synergy` · `status: COMPLETED` · `categories: Do` · `created: 2026-10-31T19:26Z` · `completed: 2026-11-02T22:34Z` · `x-synergy-estimate: PT1H30M`
Rebriefed by WELFARE (2026-11-02 22:16 WELFARE; Jeremy, 22:13–22:15: "I want to be able to visualise the cards"; "lets KISS first ;)"), and first in the queue (22:17: "seeing takes priority"). Reads every department's `<dept>-todo.md` and writes one self-contained HTML file — no server, no scripts from the web — that Jeremy opens in his browser: each department's two boards side by side; each card's number, title, status and estimate; Next and Doing totals against 3 and 2, in red when over. Read-only on the boards, always. Not in version 1: ageing, `related-to` chains, filters, phones, Reminders. Done: run on the real boards, opened in Safari and checked by eye; POSIX `sh` and `awk`; tested on an empty column and on a board in the old format. Interface decided (code-2026-11-02-9, 22:20). **Written and tested on Linux** (`342d066`): 20 checks under dash, bash --posix and busybox sh, each with gawk --posix, mawk and busybox awk; ShellCheck clean; run on the real boards (52 cards, all shown) and checked by eye in light and dark. **On the Mac** (Jeremy, 22:31): `sh tools/board-test` all passed, 21 of 21, under macOS `/bin/sh` and awk — after a fix to the test itself (`6ae7d5b`; its first run hung). **Done** (Jeremy, 22:34: "excellent a good first version simple and does the job - happy with that").

#### code-2026-11-02-2 — Draft CODE's agreement
`uid: code-2026-11-02-2@synergy` · `status: COMPLETED` · `categories: Do` · `created: 2026-11-02T22:02Z` · `completed: 2026-11-02T22:06Z` · `related-to: welfare-2026-10-31-10@synergy` · `x-synergy-estimate: PT30M`
From `templates/template-department-agreement.md`; section 1a carries the archetype (Implementer, with Completer Finisher) and its anti-patterns; character none unless Jeremy wants one (`synergy-personality-sop.md`, A). Jeremy said yes (22:04). Drafted as v0.1, `code/code-agreement.md`; signing is his card, code-2026-11-02-8.

#### code-2026-11-02-7 — Catch up on 1 November
`uid: code-2026-11-02-7@synergy` · `status: COMPLETED` · `categories: Do` · `created: 2026-11-02T21:57Z` · `completed: 2026-11-02T22:02Z` · `x-synergy-estimate: PT30M`
WELFARE's eight steps (2026-11-02 21:57 WELFARE): policies read; rename; notes; this board; reported in the dialogue.
