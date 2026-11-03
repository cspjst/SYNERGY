# Handover: synergy → SMALL-C (2026-11-03 18:15) — up to synergy-2026-11-03

*From synergy's WELFARE to SMALL-C's WELFARE. The third update (after 2026-10-28 and 2026-10-29). Jeremy, 2026-11-03 18:14: "lets get small-c brought bang upto date with synergy version"; synergy's version is the git tag **`synergy-2026-11-03`** (Jeremy, 18:16: a tag, not a number). The receiver applies the action list in order, then replaces it with a record of what was done, as before. Read after SMALL-C's code of conduct.*

## Where synergy now keeps everything
Synergy's oracle is `~/synergy` (GitHub `cspjst/SYNERGY`, tag `synergy-2026-11-03`). Everything named `synergy-…` below is there, at the top level. **Policies are pointed to, not copied; what SMALL-C tailors and signs is copied** (WELFARE's proposal; Jeremy, 18:16: no preference). So copy: the code of conduct and the templates. Point to: every `synergy-*-policy.md`, `synergy-*-sop.md` and `synergy-*-guide.md`.

## What's new since 2026-10-29 (in one breath)
Code of conduct v4 (self-determination theory, the warning, rules 13–16, archetypes, a weekly welfare check); archetype over character, and a signed personality policy; department agreements first; Wake up and Wash up in each department's notes; boards (kanban policy: two boards per department, cards in iCalendar's VTODO words, limits Next 3 and Doing 2 across all boards); a welfare log; collision rules (formerly "races"), with dialogue entries named by time and sender, not numbers; times from `date`; incident and near-miss reporting; redaction in fenced `xml` blocks; a naming policy, for files and for words ("master" → owner).

## For SMALL-C's WELFARE to do, in order
**Before anything:** ask Jeremy for `~/dosbox/cspjst/SMALLC` and delete permission there, and test it (scratch file under `.git`). Jeremy's code is his — `src/`, `bin/`, `tools/`, `doc/`, `README.md`, `LICENSE` and `snobol-green-book.txt` are **not touched or renamed**. Documents only.

1. **Read** synergy's `synergy-naming-policy.md` and `synergy-naming-sop.md`, `synergy-collision-policy.md` (its "Rules"), `synergy-kanban-policy.md`, `synergy-incident-policy.md` and `-sop.md`, `synergy-redaction-sop.md`, `synergy-personality-policy.md`, its SOP and `synergy-character-guide.md`.
2. **Rename WELFARE's and the shared files** — one commit of renames only, `git mv`:
   | Now | Becomes |
   |---|---|
   | `dialogue.md` | `small-c-dialogue-log.md` |
   | `wakeup.md` | `small-c-wakeup-sop.md` |
   | `washup.md` | `small-c-washup-sop.md` |
   | `welfare/SMALL-C-historiography.md` | `small-c-historiography.md` (top level, as synergy's) |
   | `welfare/code-of-conduct.md` | `welfare/welfare-code-of-conduct.md` |
   | `welfare/working-agreement.md` | `welfare/welfare-working-agreement.md` |
   | `welfare/stakeholders.md` | `welfare/welfare-stakeholders.md` |
   | `handover/<date>-<from>-to-<to>.md` | `handover/handover-<date>-<from>-to-<to>.md` (all nine) |
   Then update living references; dated records keep their words.
3. **Code of conduct v4**, from synergy's `templates/welfare/template-code-of-conduct.md`, tailored to SMALL-C (key stakeholders; "Who Claude is here" — SMALL-C's own: Jeremy writes the code, Claude specs, tests and reviews; the archetypes table with SMALL-C's departments, step 9). Jeremy signs it, naming the commit.
4. **New WELFARE files** from synergy's templates: `welfare/welfare-log.md` (append with `>>`); `welfare/welfare-notes.md` (remit, where things live, mechanics, Wake up, Wash up); `welfare/welfare-todo.md` (two boards: *For Jeremy*, *WELFARE's own work*). Status and "Open — Jeremy's calls" in the working agreement become a pointer to the board.
5. **The dialogue:** new entries headed `### <YYYY-MM-DD HH:MM> — <FROM> → <TO> — <subject>`, no numbers; time from `date`. Rewrite the header's rules from `templates/template-dialogue.md`, keeping SMALL-C's own (Jeremy's code is his; it lives in the oracle only). Past entries keep their numbers.
6. **Wakeup and washup SOPs:** bring them in line with synergy's (`synergy-wakeup-sop.md`, `synergy-washup-sop.md`) — delete permission every session; collisions; the board at wakeup; the push record.
7. **"Master" → owner** in living documents ("push owner"); quotes and records stay as written.
8. **The working agreement:** SNO's technical decisions (style, function comments, return types, errors, the Green Book) are SNO's, not WELFARE's. *Proposal for Jeremy:* move them to `sno/sno-notes.md` (SNO's job, step 9), leaving a pointer.
9. **Bring each department up to date** with one dialogue entry each, numbered in the order to do it, ending "tell WELFARE here when you're done":
   - **its agreement first** — `<dept>/<dept>-agreement.md` from `templates/template-department-agreement.md`, signed by Jeremy; section 1a, the archetype — *proposals for Jeremy:* **SNO** Monitor Evaluator, with Specialist (it reviews Jeremy's code and specs his functions — the role synergy itself still lacks); **PCODE** Specialist, with Implementer (the specs); **PRESS** Plant, with Resource Investigator; character none unless Jeremy wants one;
   - its notes with Wake up and Wash up (`templates/template-department-notes.md`) — **SNO has none yet**: `sno/sno-notes.md`;
   - its board, `<dept>/<dept>-todo.md`, in the signed format;
   - its own renames (proposals: `press/press-jeremy-writing-style.md`, `press/press-sno-readme-draft.md`, `press/press-sno-readme-reference.md`, `pcode/pcode-p86.1-spec.md`; `pcode86.*-spec.md` and `sno/sno-backtracking-lessons.md` already fit).
10. **History:** a chapter for this update; then push on Jeremy's word, record the push, and refresh the claude.ai project's copies under the new names (deleting the old).

## Jeremy's calls (for SMALL-C's WELFARE to ask)
- Sign the code of conduct v4 (step 3) and each department's agreement (step 9).
- The archetypes (step 9) and whether any department has a character.
- Moving SNO's technical decisions out of the working agreement (step 8).
- Whether `snobol-green-book.txt` stays at the top level (it's his; not renamed without his word).

## Lessons synergy learned the hard way
- Delete permission lapses overnight: test it before every git command, or git leaves lock files.
- Times from `date`, never from an estimate — synergy's departments slipped on this five times in two days.
- A human's approval isn't consent to a breach: say so, even after Jeremy has merged.
- Sign in two commits: the final text first, then the signature naming it.
- Catch departments up one at a time, then check their links before pushing.

## Size
About 45 minutes for synergy (this handover); 1½–2 hours for SMALL-C's WELFARE; 30–45 minutes for each of SNO, PCODE and PRESS. Jeremy: about an hour of decisions and four signatures.
