# Kanban — policy

*Owned by synergy's WELFARE; for every project. Why the human's work is kept on boards, and the rules the boards follow. **Draft v0.2, 2026-11-01** — started at Jeremy's request (21:00: "next i would like to develop kanban policy"); his answers of 21:06 are in; one question remains before it's signed. Builds on what's already agreed (2026-10-31 19:16–19:23): a Markdown kanban per department, written only by its department, limits counted across all boards.*

## Purpose
To keep the human's load **visible**, **bearable** and **moving** — welfare first. The boards are for what only the human can decide, do or read; they are not a record of the departments' own work, which lives in their notes.

## Principles
1. **Make the work visible.** What can't be seen can't be managed: every card the human owes is on a board, and nowhere else (Anderson, 2010; Benson & DeMaria Barry, 2011). One board per department; one combined view (`tools/board`, or WELFARE's report at wakeup).
2. **Limit work in progress.** **Next at most 3, Doing at most 2 — across all boards together**, because the human's load is one load. Fewer things at once means each finishes sooner: average time in the system equals work in progress divided by throughput (Little, 1961). And every switch between tasks has a cost (Rubinstein, Meyer & Evans, 2001). The limit caps load; it isn't a target.
3. **Pull, don't push.** Only the human moves a card into Next or Doing. Departments add cards to Waiting for you, and move them only when he says (Anderson & Carmichael, 2016).
4. **Writing it down frees the mind.** Unfinished goals keep intruding on thought until there's a plan for them; making the plan — even without doing it — lets them rest (Masicampo & Baumeister, 2011). A card is that plan: the human needn't hold the promise in his head, because the record holds it. That's the board's welfare job.
5. **Make progress visible.** Small, visible wins are among the strongest everyday motivators at work (Amabile & Kramer, 2011). **Done this week** stays on show until the weekly welfare check clears it.
6. **Watch the age of cards — a garbage collector.** A card that waits a long time is a signal — not of failure, but that it may not matter, or is too big (Vacanti & Coleman, 2020: "work item age"). Each card says when it was added. **At each weekly welfare check, every card waiting more than 14 days is raised: keep, drop, or pull into Next** (Jeremy, 21:06: "ageing must be addressed at some sort of timed review a sort of garbage collector if you will").
7. **"No" is a valid outcome.** A card can be dropped, into its own **Dropped** column, with the human's words and the reason (21:06: "own column pls"). A board that only grows becomes a weight. Dropped is cleared with Done at the weekly check.
8. **Make the policies explicit.** This file, the card format and the labels are the rules; everyone — human, departments, a new chat — reads the same ones (Anderson & Carmichael, 2016).
9. **Review regularly.** The weekly welfare check (code of conduct, rule 16) looks at the combined board: its size, the oldest cards, whether the limits held, and what could be dropped.
10. **Evolve, don't redesign.** Start from what works; change one rule at a time, recorded and signed (Anderson, 2010: "start with what you do now").
11. **One sitting per card.** A card should fit one sitting; a bigger one is split into cards that do (21:06: "yes split").
12. **Cards use an open standard's vocabulary.** There's no standard format for kanban cards; the nearest open standard for a task is iCalendar's to-do, VTODO (RFC 5545), in its XML form xCal (RFC 6321). Synergy adopts its property names and values, **written in Markdown** (21:06: "yes adopy RFC 6321 but as md") — so cards read well on GitHub, and a tool can export them to `.ics` for any calendar or reminders app.

## The board
- **Columns, and their RFC 5545 status** (limits held at 3 and 2: Jeremy, 21:06, "yes"):
  | Column | `status` | Note |
  |---|---|---|
  | Waiting for you | `NEEDS-ACTION` | |
  | Next (≤3 overall) | `NEEDS-ACTION`, with `priority: 1` | RFC 5545 has no status for "next"; priority 1 is its highest |
  | Doing (≤2 overall) | `IN-PROCESS` | |
  | Done this week | `COMPLETED` | cleared at the weekly check |
  | Dropped | `CANCELLED` | with the reason; cleared at the weekly check |
- **A card, in Markdown, with xCal's property names** — a heading, then one line of properties, then the description:
  ```
  #### welfare-2026-11-01-7 — The kanban policy's questions
  `uid: welfare-2026-11-01-7@synergy` · `status: NEEDS-ACTION` · `categories: Decide` · `created: 2026-11-01T21:00Z` · `x-synergy-estimate: PT5M`
  Why it matters; any proposal, labelled.
  ```
  - `uid` — `<dept>-<date>-<n>@<repo>`, unique across boards (it settles "say whose card");
  - `categories` — **Decide**, **Do** or **Read**;
  - `created` — ISO 8601, UTC; `completed` when done;
  - `related-to` — another card's `uid`, where one depends on another;
  - `x-synergy-estimate` — roughly how long, as an ISO 8601 duration (`PT5M`, `PT2H`). RFC 5545 allows `x-` properties for extensions.
- **Who writes:** only the board's department, on the human's word; the human never edits a board himself (one writer per file; no document windows).
- **Files:** `<dept>/<dept>-todo.md`, from `templates/template-todo.md`.

## Questions for Jeremy before he signs
1. ~~The limits~~ "yes" — 3 and 2 (21:06).
2. ~~Ageing~~ a timed review, "a sort of garbage collector": weekly, over 14 days (21:06).
3. ~~Dropped cards~~ "own column pls" (21:06).
4. ~~Card size~~ "yes split" (21:06).
5. **The departments' own work** — "pls to discuss this" (21:06): stay in their notes, as now — or should each department keep a board of its own work too, so you can see what it's doing?

## References
- Ohno, T. (1988). *Toyota Production System: Beyond Large-Scale Production.* Productivity Press. (Kanban's origin.)
- Anderson, D. J. (2010). *Kanban: Successful Evolutionary Change for Your Technology Business.* Blue Hole Press.
- Anderson, D. J., & Carmichael, A. (2016). *Essential Kanban Condensed.* Lean Kanban University Press.
- Vacanti, D., & Coleman, Y. (2020). *The Kanban Guide.* ProKanban.org.
- Benson, J., & DeMaria Barry, T. (2011). *Personal Kanban: Mapping Work, Navigating Life.* Modus Cooperandi Press.
- Little, J. D. C. (1961). A proof for the queuing formula L = λW. *Operations Research*, 9(3), 383–387.
- Rubinstein, J. S., Meyer, D. E., & Evans, J. E. (2001). Executive control of cognitive processes in task switching. *Journal of Experimental Psychology: Human Perception and Performance*, 27(4), 763–797.
- Masicampo, E. J., & Baumeister, R. F. (2011). Consider it done! Plan making can eliminate the cognitive effects of unfulfilled goals. *Journal of Personality and Social Psychology*, 101(4), 667–683.
- Amabile, T., & Kramer, S. (2011). *The Progress Principle.* Harvard Business Review Press.
- Desruisseaux, B. (ed.) (2009). *Internet Calendaring and Scheduling Core Object Specification (iCalendar).* RFC 5545 — VTODO, STATUS, PRIORITY, CATEGORIES, RELATED-TO, x- properties. https://www.rfc-editor.org/rfc/rfc5545
- Daboo, C., Douglass, M., & Lees, S. (2011). *xCal: The XML Format for iCalendar.* RFC 6321. https://www.rfc-editor.org/rfc/rfc6321
- Synergy: `welfare/welfare-working-agreement.md` (2026-10-31 19:16–19:23); `welfare/welfare-code-of-conduct.md` (rule 16); `templates/template-todo.md`.
