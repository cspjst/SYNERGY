# <PROJECT> — dialogue between departments

*Owned by WELFARE; every department may append. For questions, notices and replies between departments; a handover passes work or ownership.*

## How it works
- **Append only.** Newest at the bottom. Never edit or delete an entry. Append in one write with the shell's `>>` — never read the file, change it and write it back.
- **Each entry is headed** `### <YYYY-MM-DD HH:MM> — <FROM> → <TO> — <subject>`: the date, time and sender are its name; there are no numbers, so two departments writing at once can't collide. Reply with "Re <date> <time> <sender>".
- **Each entry ends with a status** — open, answered or closed. Only the department that opened an entry closes it, with an entry of its own.
- **Before writing:** test delete permission and check git isn't busy (`operating-model.md`, "Preventing races"); append; read it back; commit as `Claude-<PROJECT>-<DEPT>`, staging named paths only. Never while <HUMAN> has it open.
- **Pushing:** WELFARE alone pushes, on <HUMAN>'s word, and records each push here.
- **Read it** at the start of every session and before leaving one. A chat speaks only when <HUMAN> writes to it: <HUMAN> says "check the dialogue".
- **Decisions stay <HUMAN>'s.** A question that's theirs is marked "<HUMAN>'s call".

## Entries
