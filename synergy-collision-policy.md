# Collisions — policy

*Owned by synergy's WELFARE; for every project. What happens when two writers — agents, humans or their tools — change or read the same thing at once, and how synergy prevents it. **Draft v0.2, 2026-11-01 21:45** (v0.1 21:30; v0.2: Jeremy's answers, the rules moved in) — started while Jeremy talks with PRESS (21:28: "in my absence work on a race policy ... we should rename it something like file collision rather than race conditions"). It turns the rules in `synergy-operating-model.md` ("Preventing collisions", 2026-10-31) into a policy, with evidence. Jeremy's answers are under "Decided".*

## Why "collision"
Computing calls these *race conditions* — a term from 1950s switching circuits, where two signals "race" each other and the result depends on which arrives first (Huffman, 1954). "Race" there means a contest of speed, and the term isn't on the Inclusive Naming Initiative's lists (checked 2026-11-01). Synergy still prefers **collision**, for clarity rather than offence: it says what happens to the work, and a newcomer can't misread it. The old term is kept as an alias, so that searches for "race" still find this policy.

## Purpose
No write is lost, no name is used twice, and nobody acts on an out-of-date copy — however many agents and humans are working.

## The collisions synergy has met — named by what goes wrong
*The names follow database concurrency theory, where these anomalies were first catalogued (Berenson et al., 1995).*
1. **Lost update.** Two writers read a file, each changes its copy, and the second save wipes out the first. *Met:* the Claude app's document window saving over newer files (2026-10-27, 2026-10-31).
2. **Duplicate name.** Two writers each pick "the next number" from the same stale read. *Met:* dialogue entries 33, 34, 35 and 39, each written twice (2026-10-31).
3. **Stale read.** Someone acts on a copy older than the truth. *Met:* the friend's AI reading the sandpit code before its amendments were pushed (2026-10-29); the project's copies lagging the oracle.
4. **Interleaved tools.** Two git commands at once fight over git's own lock and index. *Met:* lock files left behind (2026-10-28 onwards).

## Principles
1. **One writer per file.** Most collisions can't happen if only one party ever writes a file — the single-writer principle (Kleppmann, 2017). Others send changes by the dialogue or a handover.
2. **Shared files are append-only logs.** Where several must write — the dialogue, the welfare log — they only *add*, in one write (the shell's `>>`), never read-change-rewrite. An append-only log is how systems from databases to git keep many writers safe (Kleppmann, 2017).
3. **Names that can't collide.** Entries in shared files are named by **time and writer**, not by a counter: two writers can't hold the same minute *and* the same name. It's the principle of Lamport's logical clocks — order by time, break ties by the writer's identity (Lamport, 1978).
4. **Check before you write — optimistic concurrency.** Read the file's modification time first; write only if it's unchanged; if it has changed, read again and merge (Kung & Robinson, 1981). Then **read it back**, at once and after a pause.
5. **One tool at a time.** Before any git command, look for git's lock: under a minute old, wait and retry; older, it's left over — remove it and say so.
6. **No document windows on shared files** while agents work. Humans look through tools that can't save — GitHub, Quick Look.
7. **Publish before inviting a read; sign the version you mean.** A stale read is prevented by pushing first, and by every signature naming the text it signs.
8. **One push owner.** Only WELFARE pushes to the backup, so the public copy changes in one place, in one order.
9. **Every collision is an incident.** Contained, reported and learned from under `synergy-incident-sop.md`.

## Rules
*Moved here from `synergy-operating-model.md` on 2026-11-01 (Jeremy, 2026-11-01 21:40: "1. keep `synergy-collision-policy.md` ... 2. yes rules in one place long pointers! ... 3. replace all occurences of master with owner ... 4. yes youre doing that as i type"), numbered as they were there. The principles above are why; these are what every department does.*
*Jeremy, 2026-10-31 18:19: "we must pin down race prevention and it must be one of the earliest jobs for a bootstrap chat". Races seen so far: the app's document window saving over newer files (2026-10-27, 10-31); a friend's AI reading the sandpit code before its amendments were pushed (10-29); dialogue entries 33, 34, 35 and 39 numbered twice by departments writing minutes apart (10-31).*

1. **One writer per file.** Only a file's owner writes it; others send changes through the dialogue or a handover (principle 3).
2. **Shared files are append only** — `synergy-dialogue-log.md`, `welfare/welfare-log.md`. Append in one write with the shell's `>>`. Never read the file, change it in memory and write the whole thing back: two writers doing that at once lose one of the writes.
3. **No sequence numbers in shared files.** An entry is identified by its date, time and sender — `### 2026-10-31 18:20 — WELFARE → PRESS — <subject>` — and referred to the same way ("Re 2026-10-31 18:14 PRESS"). Two departments can't take the same minute *and* the same name.
4. **One git at a time.** Before any git command: test delete permission (create and remove a scratch file under `.git`), and look for `.git/index.lock`. Under a minute old: another git is working — wait and retry. Older: left over — remove it and say so. Stage named paths only.
5. **Read back every write**, at once and after a pause; check the modification time before writing a file anyone else might have open.
6. **Human tools:** no document windows or editors on the repository's files while agents work. To look, use GitHub or Quick Look, which can't save.
7. **Publishing:** push before asking anyone outside to read; sign the version you mean.
8. **One push owner:** WELFARE (formerly "push master").
9. **Say whose card:** each department's board names its cards `<date>-<n>`, so the names repeat across boards; refer to a card with its board — "CODE todo 2026-10-31-1" (PRESS and CODE, 2026-10-31 19:30–19:31).
10. **A human's approval isn't consent to a breach** (2026-11-01 20:18): when Claude sees a breach, it names it as a breach, even in something a human has already merged or approved — humans miss things; that's what the second pair of eyes is for.

## Decided (Jeremy, 2026-11-01 21:40)
1. **The name:** "keep `synergy-collision-policy.md`".
2. **One place for the rules:** "yes rules in one place long pointers!" — the rules above; the model keeps a pointer.
3. **"Master" → "owner":** "replace all occurences of master with owner" — "push owner" in living documents; quotes and dated records keep "push master" (`synergy-naming-policy.md`, rule 14).
4. **A naming check for old terms:** done — `synergy-naming-policy.md`, rules 11–15.

Awaiting Jeremy's signature.

## References
- Huffman, D. A. (1954). The synthesis of sequential switching circuits. *Journal of the Franklin Institute*, 257(3), 161–190; 257(4), 275–303.
- Berenson, H., Bernstein, P., Gray, J., Melton, J., O'Neil, E., & O'Neil, P. (1995). A critique of ANSI SQL isolation levels. *Proceedings of ACM SIGMOD*, 1–10.
- Kung, H. T., & Robinson, J. T. (1981). On optimistic methods for concurrency control. *ACM Transactions on Database Systems*, 6(2), 213–226.
- Lamport, L. (1978). Time, clocks, and the ordering of events in a distributed system. *Communications of the ACM*, 21(7), 558–565.
- Kleppmann, M. (2017). *Designing Data-Intensive Applications.* O'Reilly. (Single-leader writes; logs.)
- Inclusive Naming Initiative. *Word lists* (tiers 1–3 and "no change"). https://inclusivenaming.org/word-lists/inclusive-naming-word-lists-v1.0
- Synergy: `synergy-operating-model.md` (a pointer here); `synergy-incident-policy.md`; `welfare/near-misses/`.
