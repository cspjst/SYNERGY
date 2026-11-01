# Collisions — policy

*Owned by synergy's WELFARE; for every project. What happens when two writers — agents, humans or their tools — change or read the same thing at once, and how synergy prevents it. **Draft v0.1, 2026-11-01** — started while Jeremy talks with PRESS (21:28: "in my absence work on a race policy ... we should rename it something like file collision rather than race conditions"). It turns the rules in `synergy-operating-model.md` ("Preventing collisions", 2026-10-31) into a policy, with evidence. The questions at the end are Jeremy's before it's signed.*

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
8. **One pusher.** Only WELFARE pushes to the backup, so the public copy changes in one place, in one order.
9. **Every collision is an incident.** Contained, reported and learned from under `synergy-incident-sop.md`.

## Questions for Jeremy before he signs
1. **The name:** "collision" — `synergy-collision-policy.md`, and "Preventing collisions" in the model — or "file collision", or another?
2. **The model's section:** move its rules here, leaving a pointer, so the rules live in one place?
3. **"Push master"** — your own phrase (2026-10-27 21:19: "we need a push master"), which stays as you said it. But "master" is on the Inclusive Naming Initiative's tier 1 ("replace immediately"). For the living documents: **"the pusher"**, **"push owner"**, or keep "push master"?
4. ~~A naming check for old terms~~ Done: `synergy-naming-policy.md`, rules 11–15 (Jeremy, 21:35: "pls update the naming policy with this new information").

## References
- Huffman, D. A. (1954). The synthesis of sequential switching circuits. *Journal of the Franklin Institute*, 257(3), 161–190; 257(4), 275–303.
- Berenson, H., Bernstein, P., Gray, J., Melton, J., O'Neil, E., & O'Neil, P. (1995). A critique of ANSI SQL isolation levels. *Proceedings of ACM SIGMOD*, 1–10.
- Kung, H. T., & Robinson, J. T. (1981). On optimistic methods for concurrency control. *ACM Transactions on Database Systems*, 6(2), 213–226.
- Lamport, L. (1978). Time, clocks, and the ordering of events in a distributed system. *Communications of the ACM*, 21(7), 558–565.
- Kleppmann, M. (2017). *Designing Data-Intensive Applications.* O'Reilly. (Single-leader writes; logs.)
- Inclusive Naming Initiative. *Word lists* (tiers 1–3 and "no change"). https://inclusivenaming.org/word-lists/inclusive-naming-word-lists-v1.0
- Synergy: `synergy-operating-model.md` ("Preventing collisions"); `synergy-incident-policy.md`; `welfare/near-misses/`.
