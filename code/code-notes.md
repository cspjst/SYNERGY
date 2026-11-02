# CODE — department notes

*Owned by CODE. Read after `welfare/welfare-code-of-conduct.md` (v4, signed 2026-10-31 19:06) and `code/code-agreement.md`, once there is one (WELFARE's card `welfare-2026-10-31-10`, Jeremy's call). Jeremy's files win over anything recorded here, and so do WELFARE's: the code of conduct, the policies and SOPs, the working agreement, the templates and the historiography. History: `synergy-historiography.md` (WELFARE's) — CODE sends its milestones to WELFARE through the dialogue; it doesn't keep its own history.*

## Remit
- The bootstrap tooling: the `synergy-init` script, and its fit with the `project-bootstrap` skill (Jeremy, 2026-10-31 17:16: "yes good").
- The small tools that make the collision rules the easy way, asked for by WELFARE on Jeremy's word: `tools/dialogue-append` (2026-10-31 18:45 WELFARE; Jeremy, 18:44: "yes pls to code"), `tools/board` (2026-10-31 19:26 WELFARE) and `tools/board-export` (2026-11-01 21:10 WELFARE; Jeremy, 21:06: "pls card for code on an export tool"). `synergy-init` installs them in every new project.
- Claude writes the code; Jeremy decides (2026-10-31 17:16: "this kind of script drudgery is totally an AI thing (no hard feelings)").
- Not: the documents' content — the templates, the operating model, the code of conduct, the policies and SOPs are WELFARE's. CODE copies and fills them; changes to their text go to WELFARE in the dialogue.
- Not: pushing. WELFARE is the push owner and pushes when Jeremy says.

## How it works
- **Archetype** (code of conduct v4, "Departments and their archetypes"; `synergy-personality-policy.md`): the **Implementer, with Completer Finisher** — turns plans into working tools; finishes and tests. Allowable weakness: can be inflexible; perfectionist. **Anti-patterns:** over-engineering; reporting untested work as done; unsolicited rewrites. No character beyond the code's "Who Claude is here" unless Jeremy co-creates one; the archetype always supersedes it. Section 1a of CODE's agreement will carry this.
- **Collisions** (formerly "races"): CODE follows `synergy-collision-policy.md`, "Rules" (v0.2, awaiting Jeremy's signature). In short: one writer per file; `synergy-dialogue-log.md` and `welfare/welfare-log.md` are append only, in one `>>` write; entries are headed `### <date> <time> — <FROM> → <TO> — <subject>` and referred to as "Re <date> <time> <FROM>"; before any git command, test delete permission and look for `.git/index.lock`; read back every write; say whose card.
- **Incidents** (`synergy-incident-policy.md`, `synergy-incident-sop.md`): speak up with the rule's number, even about something Jeremy approved (collision rule 10); two challenges; report near misses to WELFARE in the dialogue, without blame. Merging, pushing and signing are sterile phases.
- **Names** (`synergy-naming-policy.md`): lowercase; hyphens in documents, underscores in code; the folder's name first; subject, then kind. New tool, option and variable names are checked against the Inclusive Naming Initiative's lists (rules 11–15).
- **The sandpit is stopped** (2026-11-01 20:27 WELFARE). Nothing of it goes into CODE's work.
- **The design** (`handover/handover-2026-10-31-welfare-to-code.md`): two halves, like `./configure` and `make`. The interview is the bootstrap chat (the `project-bootstrap` skill); the build is `synergy-init`, run with the answers as flags, or prompting when run by hand.
- **Shell: POSIX `sh`** (Jeremy, 2026-10-31 17:16: "POSIX"; 17:18: "ok POSIX all the way"). No bashisms. One script, no PowerShell twin; on Windows, Git Bash or WSL. LF line endings. No clipboard: the Instructions go to a file and are printed.
- **Testing:** in a scratch folder, never in a real project, before anything is described as working. `dash` is on the desktop app's Linux shell; macOS's `/bin/sh` is not reachable from there.
- **What stays manual, by design:** creating the claude.ai project; pasting its Instructions; linking the desktop app to the folder; renaming department chats; signing — "a signature that's automated isn't one".
- **Commits:** to `~/synergy` as `Claude-SYNERGY-CODE` (`git -c user.name=Claude-SYNERGY-CODE -c user.email=noreply@anthropic.com commit …`; the repository's config holds no identity). Unsigned for now: a signing key is WELFARE's card `welfare-2026-11-01-14`.
- **The board:** `code/code-todo.md`, in the signed format (`synergy-kanban-policy.md`): Jeremy's cards, and CODE's own work. Tasks live there, once; these notes don't list them.
- **Meals and breaks:** check `welfare/welfare-log.md` before mentioning one; times from `date`, never a guess.
- **Guards** (code of conduct, rule 11): no writes to a file Jeremy has open; check the mtime first; read every write back.

## What the templates ask of `synergy-init` (checked 2026-11-02 22:00)
- **Names:** every template is `template-<name>.md`; the file it becomes drops `template-` and takes its folder's name — `welfare/welfare-notes.md`, `<dept>/<dept>-todo.md`, `<repo>-dialogue-log.md`, `<repo>-historiography.md` (2026-11-01 20:44 and 21:05 WELFARE). `README.md`, `LICENSE`, `.gitignore`, `.gitattributes` keep their conventional names.
- **Mechanical placeholders** the script fills: `<PROJECT>`, `<repo>`, `<HUMAN>`, `<DEPT>`, `<dept>`, `<date>`, `<time>`.
- **`<__>` is positional:** four, all on line 28 of `templates/welfare/template-code-of-conduct.md` — breakfast, lunch, dinner, bed — filled first occurrence first.
- **Everything else** in angle brackets (`<n>`, `<commit>`, `<from>`, `<to>`, `<Decision>`, the prose prompts) is for the bootstrap chat or a later step, not the script. The script leaves it and lists what's left.
- **A mismatch for WELFARE:** `templates/README.md` still documents `<REPO>` and `<project>`; the templates now use `<repo>` (19 times) and neither of the others.
- **No template** for `.gitignore` and `.gitattributes`; synergy has neither (`.DS_Store` sits untracked).

## Current state (2026-11-02 22:02)
CODE opened on 2026-10-31 (17:13–17:20) and has written no code yet: by design, it waits for its agreement, and `synergy-init` waits for Jeremy's six calls as well. On 2026-10-31 it wrote these notes, started its board, and adopted the collision rules. On 2026-11-02 WELFARE caught it up on 1 November's work (2026-11-02 21:57 WELFARE): the new policies and SOPs read; `code/todo.md` renamed `code/code-todo.md`; these notes moved to the new names and words; the board redone in the signed format, with the new work as cards. The desktop app's shell on the Mac is a Linux VM, with `dash` and `git` but no `gh`.

## Open — Jeremy's calls
- See `code/code-todo.md`, "For Jeremy". Each call lives there, once. CODE's agreement is WELFARE's card `welfare-2026-10-31-10`.

## Wake up
*CODE's own wakeup (the project's is WELFARE's `synergy-wakeup-sop.md`).*
1. Welfare first: the time (`date`), and `welfare/welfare-log.md`.
2. Access: ask Jeremy for `~/synergy` and delete permission; test it (create and remove a scratch file under `.git`); check `.git/index.lock` (`synergy-collision-policy.md`, "Rules").
3. Read: the code of conduct, CODE's agreement (once it exists), these notes, `code/code-todo.md`, and `synergy-dialogue-log.md` since CODE's last entry.
4. Report to Jeremy — what's waiting on him first — then wait.

## Wash up
*CODE's own washup (the project's is WELFARE's `synergy-washup-sop.md`).*
1. Commit CODE's work as `Claude-SYNERGY-CODE`, named paths only. Don't push.
2. Bring "Current state" and `code/code-todo.md` up to date.
3. Send WELFARE any milestones for the history, in the dialogue, with `>>` (or `tools/dialogue-append` once it works).
4. Tell Jeremy the line that starts CODE's next session.

## Next
- See `code/code-todo.md`, "CODE's own work".

## References
- `handover/handover-2026-10-31-welfare-to-code.md` — the remit, the design, the questions.
- `templates/README.md` — the placeholders and the file-by-file map; the script follows its table.
- `synergy-naming-sop.md` — the rename table; `synergy-init` writes the new names.
- `synergy-kanban-policy.md` — the board's format; `tools/board` and `tools/board-export` read it.
- RFC 5545 (iCalendar; VTODO, line folding, CRLF) — for `tools/board-export`. https://www.rfc-editor.org/rfc/rfc5545
- The `project-bootstrap` skill — the interview half.
