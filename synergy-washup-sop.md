# Washup — leaving a chat so the next one can pick up from the oracle

*First done in synergy, 2026-10-29 19:30–19:50, at Jeremy's request: "perform a washup procedure ... so that I can leave this chat where it is an return at some point in the future and you will be able to start it up again from ~/synergy"; made generic for every project (2026-10-31 17:03: "pls genericise"). Its complement is `wakeup.md`. Where this project keeps things, and how WELFARE commits, signs and pushes here, are in `welfare/welfare-notes.md`.*

**This is the project's washup, and only WELFARE runs it** (Jeremy, 2026-10-29 19:44: "*ONLY* welfare can wakeup and washup"); WELFARE alone pushes, too. **Every other department washes up from the "Wash up" section of its own notes** — commit its work, bring its notes up to date, send its milestones to WELFARE in the dialogue — and doesn't push or write the history (Jeremy, 2026-10-31 18:14, 18:19).

## When
- Before leaving a chat for a while, before a planned compaction, or when the human says "washup".
- Not as a substitute for writing things down as they happen (principle 1) — a washup catches what slipped through.

## The steps
1. **Welfare first.** Is it a sensible hour; has the human eaten? A washup can wait for dinner.
2. **Check access.** The oracle folder, and delete permission there (create and remove a scratch file under `.git`); the keys folder. Ask again if any has lapsed.
3. **Commit WELFARE's work**, signed if WELFARE signs. Stage named paths only. Leave other departments' and the human's uncommitted work alone, and their notes too — departments keep their own current (Jeremy, 2026-10-29 19:46: "i prefer as much departmental siloing ... as \"reasonable\" we want an effective chain of command but not one that throttles ease of use"); mention anything outstanding.
4. **Write the history.** Extend `<REPO>-historiography.md` with everything since its last chapter, while the chat still remembers it: the problem, what was tried, what the sources said, what was decided — the human's words quoted and timed, thin stretches labelled. Other departments' milestones come to WELFARE through the dialogue.
5. **Bring the working agreement up to date.** Its Status and "Open — <HUMAN>'s calls" sections, so a fresh session can trust them.
6. **Lessons into the operating model** — anything general this chat learned; into `wakeup.md` anything that changes how every session starts; into `welfare/welfare-notes.md` anything particular to this project's mechanics.
7. **Tidy the dialogue.** Close your open entries, or say why they stay open.
8. **Write the washup handover:** `handover/<date>-welfare-washup.md` — where things stand, what's waiting on whom, anything `wakeup.md` doesn't already say. Short: the documents carry the detail.
9. **Push all** — WELFARE only. Asking for a washup is the word to push (Jeremy, 2026-10-29 19:38: "yes washup implies push all"). Fetch first: if GitHub has commits the oracle hasn't (the human's from another machine, a collaborator's merged pull request), bring them in before pushing. Record the push in the dialogue with the hash.
10. **Refresh the project's copies**, at the paths its Instructions use.
11. **Verify.** Read every write back; the oracle, GitHub and the project agree; signed commits verify.
12. **Tell the human** the one line that starts the next session, e.g. *"WELFARE. Read wakeup.md in <oracle folder> and follow it."*
