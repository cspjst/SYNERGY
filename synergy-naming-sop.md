# Naming — SOP

*Owned by synergy's WELFARE; for every project. How to name a file, and how to rename one. The rules and their evidence are in `synergy-naming-policy.md`.*

## Naming a new file
1. **Which folder?** Its name comes first — at the top level, the repository's (`synergy-`).
2. **Dated record?** Then the date, `YYYY-MM-DD`.
3. **Subject**, in a word or two.
4. **Kind**, last: `-policy`, `-sop`, `-guide`, `-log`, `-notes`, `-todo`, `-agreement`.
5. **Check:** lowercase; only `a`–`z`, `0`–`9`, `-`; no version; short but clear. Code follows its language.

## Adopting a term
1. **Plain word first** — does it say what happens to the work?
2. **Check it** against the Inclusive Naming Initiative's current word lists (`synergy-naming-policy.md`, rules 11–15); note the date checked.
3. **Tier 1:** don't use it. **Tier 2 or 3:** use a clearer word if there is one. **No change:** fine.
4. **Replacing an old term:** change it in living documents only — never in quotes or dated records; give the old term once as an alias where the new one is defined; record the decision and reason in the working agreement; tell the departments in the dialogue.

## Renaming a file
1. **Sterile phase** (`synergy-incident-sop.md`): one rename at a time, nothing else in that commit.
2. `git mv` — never delete-and-recreate, so history follows the file.
3. **Update living references** — documents that describe the present — and check the new name's words ("Adopting a term"); leave dated records (history, handovers, the dialogue, settled decisions) as they were written.
4. **Search for the old name** afterwards; expect only dated records to mention it.
5. **Tell the departments** in the dialogue, and the human if the project's Instructions or a skill name the file.
6. **Refresh the project's copies**, and delete the copy under the old name.

## The migration of 2026-11 — approved (Jeremy, 2026-11-01 20:53: "top level files included pls sop approve proceed to implementation")
*Done by WELFARE, 2026-11-01: its own files and the shared ones (renames only in `3fd45fc`; references in the next commit). **Waiting:** PRESS's and CODE's files (theirs to rename, at their next session); the sandpit's two files (with Ray, once the stop is resolved).*
*Each department renames its own files (siloing); WELFARE renames its own and the shared ones. Living references updated; dated records left.*

| Now | Becomes | Whose |
|---|---|---|
| `SYNERGY-historiography.md` | `synergy-historiography.md` | WELFARE |
| `operating-model.md` | `synergy-operating-model.md` | WELFARE |
| `policy-incident.md`, `sop-incident.md` | `synergy-incident-policy.md`, `synergy-incident-sop.md` | WELFARE |
| `redaction.md` | `synergy-redaction-sop.md` | WELFARE |
| `washup.md`, `wakeup.md` | `synergy-washup-sop.md`, `synergy-wakeup-sop.md` | WELFARE |
| `connect-github.md` | `synergy-connect-github-guide.md` | WELFARE |
| `dialogue.md` | `synergy-dialogue-log.md` | WELFARE |
| `welfare/code-of-conduct.md` | `welfare/welfare-code-of-conduct.md` | WELFARE |
| `welfare/working-agreement.md` | `welfare/welfare-working-agreement.md` | WELFARE |
| `welfare/stakeholders.md`, `welfare/third-party-ai.md`, `welfare/todo.md` | `welfare/welfare-stakeholders.md`, `welfare/welfare-third-party-ai-agreement.md`, `welfare/welfare-todo.md` | WELFARE |
| `welfare/near-misses/2026-11-01-sandpit-rule-6.md` | `welfare/near-misses/near-miss-2026-11-01-sandpit-rule-6.md` | WELFARE |
| *(new)* | `welfare/welfare-incident-log.md` | WELFARE |
| `handover/<date>-….md` | `handover/handover-<date>-….md` | WELFARE |
| `sandpit/code_of_conduct.md`, `sandpit/conversation.md` | `sandpit/sandpit-code-of-conduct.md`, `sandpit/sandpit-conversation-log.md` | WELFARE — **with Ray**, as the sandpit is shared |
| `templates/…` | already `template-…`; `<REPO>-historiography.md` becomes `<repo>-historiography.md` | WELFARE |
| `press/todo.md`, `press/writer-editor-agreement.md`, `press/writing-framework.md`, `press/v2-…` | `press/press-todo.md`, `press/press-writer-editor-agreement.md`, `press/press-writing-framework.md`; `press/press-v2-…` | PRESS |
| `code/todo.md` | `code/code-todo.md` | CODE |
| `README.md`, `LICENSE`, `sandpit/README.md`, `sandpit/keys/allowed_signers` | unchanged — conventional names | — |

**Knock-ons:** the project's Instructions (they name `welfare/code-of-conduct.md`, `welfare/working-agreement.md`, `synergy/operating-model.md`) — Jeremy pastes new ones; the `project-bootstrap` skill — a new proposal; CODE's `synergy-init` design; the sandpit's guide and Ray's PRs, which name `sandpit/conversation.md`.
