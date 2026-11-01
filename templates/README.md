# Bootstrap templates

*Owned by synergy. Every template is named `template-<name>.md` (Jeremy, 2026-11-01 20:37: "I favour naming the ones in templates as template-"); the file it becomes drops the prefix. Masters for starting a new project with Claude, per `synergy-operating-model.md`. Copy them into a new project at bootstrap; from then on the copies belong to that project. Synergy's WELFARE is the original; every project's WELFARE is bootstrapped from it.*

## Placeholders
- `<PROJECT>` — the project's name in capitals; `<project>` — lower case where a path needs it.
- `<REPO>` — the repository's name, as GitHub has it (e.g. `SMALL-C`, `SYNERGY`); the historiography is named after it (Jeremy, 2026-10-28 19:25).
- `<DEPT>` / `<dept>` — a department's name / its folder.
- `<HUMAN>` — the human's name (Jeremy).
- `<date>` — `YYYY-MM-DD`; `<time>` — `HH:MM`, UK local.
- `<…>` anything else — fill in or delete. Lines in *italics* starting "Guide:" are guidance; delete them once filled.

## The files, in bootstrap order
| Step | Template | Becomes, in the new project |
|---|---|---|
| 1 | `template-project-instructions.md` | pasted into the project's Instructions (Claude can't edit them) |
| 2 | `welfare/template-stakeholders.md` | `welfare/welfare-stakeholders.md` |
| 2 | `welfare/template-code-of-conduct.md` | `welfare/welfare-code-of-conduct.md` — signed by the human |
| 2 | `welfare/template-working-agreement.md` | `welfare/welfare-working-agreement.md` |
| 3 | `template-historiography.md` | `<repo>-historiography.md` (owner: WELFARE) |
| 4 | `template-department-opening.md` | the first message of each department chat |
| 4 | `template-department-notes.md` | `<dept>/<dept>-notes.md` |
| any | `template-incident-report.md` | `welfare/near-misses/<date>-<short-name>.md` — under `<repo>-incident-sop.md` |
| 4 | `template-todo.md` | `<dept>/<dept>-todo.md` — the human's to-do, one per department (WELFARE's in `welfare/`) |
| any | `handover/template-handover.md` | `handover/<date>-<from>-to-<to>.md` |
| 1 | `template-dialogue.md` | `<repo>-dialogue-log.md` at the oracle's root — race rules built in |
| 1 | `welfare/template-welfare-log.md` | `welfare/welfare-log.md` |
| 4 | `template-department-agreement.md` | `<dept>/<dept>-agreement.md` — each department's first document, signed |
| 2 | `../<repo>-washup-sop.md`, `../<repo>-wakeup-sop.md` (synergy's root) | `<repo>-washup-sop.md`, `<repo>-wakeup-sop.md` at the new oracle's root — copied as they are; they're generic |
| 2 | `template-department-notes.md` | `welfare/welfare-notes.md` — WELFARE's remit, where things live, how it commits, signs and pushes |

## Rules that come with them
- Every project has a WELFARE department, and it is the main department: it keeps the stakeholders, the code of conduct, the working agreement and the historiography (operating model, principles 7 and 8).
- Rename each department chat by hand; auto-titles aren't reliable.
- One owner per document; the header of each says who.
- Claude doesn't write to a file the human has open, and verifies every write to the human's machine by reading it back.
