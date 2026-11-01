# Wakeup — starting a chat cold from the oracle

*The complement of `washup.md`. Written for synergy (Jeremy, 2026-10-29 19:33–19:35: "its complementary wakeup.md"; "make it so") and made generic for every project (2026-10-31 17:03: "pls genericise"). A new session remembers nothing: it trusts nothing until it has checked it. Start here when the human says "wakeup", or "Read wakeup.md". Where this project keeps things, and how WELFARE commits, signs and pushes here, are in `welfare/welfare-notes.md`.*

> **Warning — document windows are dangerous** (Jeremy, 2026-10-31 17:33: "dont use document windows theyre dangerous"). A file open in the Claude app's document window, or in an editor, is saved back from its loaded copy, silently undoing a newer write — seen 2026-10-27 17:44–17:59, and again 2026-10-31 17:30. **Human:** don't keep the repository's files open there while Claude works. **Claude:** don't write to a file the human has open; read every write back, once at once and again after a pause.

**This is the project's wakeup, and only WELFARE runs it** (Jeremy, 2026-10-29 19:44: "*ONLY* welfare can wakeup and washup"). **Every other department wakes up from the "Wake up" section of its own notes** (Jeremy, 2026-10-31 18:14: "depts should dept specific wakeups and washups as well as notes"; 18:19: "sections in notes").

## The steps
1. **Welfare first.** Check the time against the code of conduct's meal times and bedtime, and `welfare/welfare-log.md` for what's already happened today; then ask how the human is — before anything else.
2. **Access, and races.** Ask the human for the oracle folder, then for delete permission there, and test it (create and remove a scratch file under `.git`) — before any git command, `git fetch` included. Then the rest of "Preventing races" in `operating-model.md`: one git at a time, appends with `>>`, entries named by time and sender. If WELFARE signs its commits, ask for the keys folder too.
3. **Read, in order:**
   1. `welfare/code-of-conduct.md` — it wins over everything else;
   2. `welfare/working-agreement.md` — its Status and "Open — <HUMAN>'s calls" first;
   3. `welfare/welfare-notes.md` — where things live, and the mechanics;
   4. the latest washup handover — `handover/<date>-welfare-washup.md`, newest date;
   5. `operating-model.md`;
   6. `<REPO>-historiography.md` — the latest chapter at least;
   7. `dialogue.md` — every entry since WELFARE's last.
4. **Check git, both ways.** `git fetch`; then what's on GitHub that isn't here (`main..origin/main` — the human's commits from other machines, collaborators' merged pull requests), what's here that isn't on GitHub (`origin/main..main`), open pull requests, uncommitted changes, and leftover `.lock` files.
5. **Check what changed while asleep.** New dialogue entries; any conversation with another AI; whether the project's copies and its Instructions still match the oracle.
6. **Check identity** (if WELFARE signs): the key file is where it should be — without reading it — and the last signed commit verifies against `allowed_signers`, with the fingerprint in the notes.
7. **Report, then wait.** Tell the human, briefly: what changed since the washup; **the combined board** — every department's `todo.md` read together (`tools/board`, when it exists), with the totals in Next and Doing against the limits; and one suggested first step. Waking up isn't permission to start work.
