# Kanban — policy

*Owned by synergy's WELFARE; for every project. Why the human's work is kept on boards, and the rules the boards follow. **Draft v0.1, 2026-11-01** — started at Jeremy's request (21:00: "next i would like to develop kanban policy"); the questions at the end are his before it's signed. Builds on what's already agreed (2026-10-31 19:16–19:23): a Markdown kanban per department, written only by its department, limits counted across all boards.*

## Purpose
To keep the human's load **visible**, **bearable** and **moving** — welfare first. The boards are for what only the human can decide, do or read; they are not a record of the departments' own work, which lives in their notes.

## Principles
1. **Make the work visible.** What can't be seen can't be managed: every card the human owes is on a board, and nowhere else (Anderson, 2010; Benson & DeMaria Barry, 2011). One board per department; one combined view (`tools/board`, or WELFARE's report at wakeup).
2. **Limit work in progress.** **Next at most 3, Doing at most 2 — across all boards together**, because the human's load is one load. Fewer things at once means each finishes sooner: average time in the system equals work in progress divided by throughput (Little, 1961). And every switch between tasks has a cost (Rubinstein, Meyer & Evans, 2001). The limit caps load; it isn't a target.
3. **Pull, don't push.** Only the human moves a card into Next or Doing. Departments add cards to Waiting for you, and move them only when he says (Anderson & Carmichael, 2016).
4. **Writing it down frees the mind.** Unfinished goals keep intruding on thought until there's a plan for them; making the plan — even without doing it — lets them rest (Masicampo & Baumeister, 2011). A card is that plan: the human needn't hold the promise in his head, because the record holds it. That's the board's welfare job.
5. **Make progress visible.** Small, visible wins are among the strongest everyday motivators at work (Amabile & Kramer, 2011). **Done this week** stays on show until the weekly welfare check clears it.
6. **Watch the age of cards.** A card that waits a long time is a signal — not of failure, but that it may not matter, or is too big (Vacanti & Coleman, 2020: "work item age"). Each card says when it was added.
7. **"No" is a valid outcome.** A card can be dropped, with the human's words and the reason recorded. A board that only grows becomes a weight.
8. **Make the policies explicit.** This file, the card format and the labels are the rules; everyone — human, departments, a new chat — reads the same ones (Anderson & Carmichael, 2016).
9. **Review regularly.** The weekly welfare check (code of conduct, rule 16) looks at the combined board: its size, the oldest cards, whether the limits held, and what could be dropped.
10. **Evolve, don't redesign.** Start from what works; change one rule at a time, recorded and signed (Anderson, 2010: "start with what you do now").

## The board
- **Columns:** Waiting for you · Next (≤3 overall) · Doing (≤2 overall) · Done this week.
- **A card:** its name (`<date>-<n>`, referred to with its board: "CODE todo 2026-10-31-1"), a one-line title, a label — **Decide**, **Do** or **Read** — why it matters, any proposal (labelled), and roughly how long it takes.
- **Who writes:** only the board's department, on the human's word; the human never edits a board himself (one writer per file; no document windows).
- **Files:** `<dept>/<dept>-todo.md`, from `templates/template-todo.md`.

## Questions for Jeremy before he signs
1. **The limits:** keep Next 3, Doing 2 — or change them?
2. **Ageing:** a card waiting more than **14 days** is raised at the weekly check — keep, drop, or pull into Next? Or another threshold?
3. **Dropped cards:** removed with a line in Done this week ("dropped — why"), or a **Dropped** column of their own?
4. **Card size:** a card should fit **one sitting**; bigger ones are split. Agree?
5. **The departments' own work:** stay in their notes, as now — or should each department keep a board of its own work too, so you can see what it's doing?

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
- Synergy: `welfare/welfare-working-agreement.md` (2026-10-31 19:16–19:23); `welfare/welfare-code-of-conduct.md` (rule 16); `templates/template-todo.md`.
