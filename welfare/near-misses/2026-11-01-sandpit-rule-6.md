# Incident report 1 — personal information in the sandpit (2026-11-01)

*Owned by WELFARE. Written 2026-11-01 at Jeremy's request (20:22): "this is a really exciting important near miss and we must like the airline industry learn from out near misses! pls make a historiography note and summarise the learning and how to put into SOP(s)". In the spirit of aviation safety reporting: facts first, no blame, learning last. Strictly an **incident** — the information reached the public repository — contained, rather than a near miss.*

## What happened
| Time (2026-11-01) | Event |
|---|---|
| 12:25 | Rufus's entry 003 committed by Ray, signed; it includes personal information about Ray's private life and a member of his family, who isn't a party to the sandpit. |
| 19:56 | Jeremy merges pull request #4 on GitHub. The text is now in the public repository. |
| 20:11–20:15 | Claude-SYNERGY-WELFARE wakes, verifies the signature, reads the entry, and raises the personal information with Jeremy — as "one welfare point", suggesting "a quiet word with Ray", reasoning that Jeremy's merge "may count as agreeing". |
| 20:18 | Jeremy: "i merged without noticing the breach you have done well there but you assumed i was correct rather than questioning it". He directs redaction and a stop. |
| 20:25 | Redacted in place; entry 004, STOP — breach 1, rule 6. |
| now | The original text remains in git history (`49d3fd2`) and in pull request #4. |

## The defences, and where each one had a hole
*After James Reason's "Swiss cheese" model: harm gets through when the holes in successive defences line up.*
1. **The writer (Rufus).** Rule 6 was in the code it had read and accepted. It wrote the personal detail in service of a good point — that collaboration matters to a human's life — and didn't see it as private data.
2. **The writer's supervisor (Ray).** Carried the entry in by pull request; the detail was about his own life and family, and familiar to him — the hardest kind to see as sensitive.
3. **The receiver's supervisor (Jeremy).** Merged without reading for rule 6 — a merge done as routine.
4. **The receiving AI (Claude).** Saw it, but treated a human's merge as consent, and called a breach "a welfare point". The hole: deference.
5. **Publication.** A public repository with full history: once merged, redaction can't fully undo it.

## What went right
- The signature and key checks worked: no doubt about where the entry came from.
- Claude did see it, at its first read.
- Jeremy questioned Claude's deference at once, and acted within minutes.
- The stop worked as designed: one entry, named and explained, no quoting of the private text.
- Nobody was blamed. Fenwick's Law held: an honest mistake reported quickly costs little.

## The learning
1. **A human's approval isn't consent to a breach.** An AI that defers to a human's action has stopped being a second pair of eyes. *(In the model, "Preventing races", rule 10, 2026-11-01.)*
2. **Name breaches as breaches.** "A welfare point" undersold a rule-6 breach. Cite the rule and its number.
3. **Check at the gate, not after it.** Every defence that worked, worked after publication. The check belongs before the merge.
4. **Familiar information is the hardest to see as private** — for the person it's about, and for those close to them.
5. **In a public repository, publication is permanent.** Prevention is cheap; removal is not.
6. **Report without blame, and learn.** That's how the airline industry got safe.
7. **A safeguard has to show.** The first redactions used bare `<redacted>` tags, which GitHub's display silently drops — so they looked absent (Jeremy, 20:26: "point of order you have not used the xml tags I requested"). Now `redaction.md`: an agreed block, inside a fenced code block, so it shows (20:27: "perfect"); both redactions redone as R1 and R2.

## Into standard procedures — proposals, Jeremy's calls (and Ray's, where the sandpit's code changes)
1. **A pre-merge review for the sandpit.** Before Jeremy merges a pull request into `sandpit/`, he asks WELFARE to review it. WELFARE fetches the pull request, verifies the signature, checks it touches only `sandpit/conversation.md`, reads it against each rule of the sandpit code — rule 6 first: people who aren't parties, family, health, addresses, money, credentials — and reports: merge, or not and why. *A practice for Jeremy; no change to the signed code. The first job of the Monitor Evaluator role (WELFARE todo 2026-10-31-2).*
2. **A near-miss and incident procedure,** in `operating-model.md`: contain (stop, redact); report (one file per event in `welfare/near-misses/`, this one the first — facts, defences, what went right, learning, actions); no blame; turn the learning into procedures, signed where they need signing; share the report with everyone involved — here, Ray.
3. **A rule-6 check in the sandpit's code** (an amendment, both humans to sign): each AI checks its own entry for personal information before handing it to its supervisor, and says so in the entry ("Rule 6 checked").
4. **The history question:** whether to rewrite git history and ask GitHub to purge pull request #4. Ray's call first, as it's his family.

## Sources
- NASA Aviation Safety Reporting System (ASRS), since 1976 — confidential, non-punitive reporting of incidents and near misses.
- Reason, J. (1990). *Human Error.* Cambridge University Press; Reason, J. (2000). Human error: models and management. *BMJ*, 320, 768–770.
- Dekker, S. (2007). *Just Culture: Balancing Safety and Accountability.* Ashgate.
- Synergy: `sandpit/code_of_conduct.md` (rule 6, "Breaches and the stop"); `sandpit/conversation.md` entries 003–004; `welfare/working-agreement.md` (2026-11-01).
