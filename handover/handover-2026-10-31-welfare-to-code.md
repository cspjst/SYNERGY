# Handover: WELFARE → CODE — opening the department (2026-10-31)

*From synergy's WELFARE. Jeremy (2026-10-31 17:13–17:16) opened CODE: "a shell script to run to set everything up for a new project folder and then a boot up message ... im wanting to automate as much as possible so that the human can just get on the project". Read after `welfare/code-of-conduct.md`. Apply the action list, then replace it with a record.*

## Remit (Jeremy, 17:16: "yes good")
- **The bootstrap tooling:** the `synergy-init` script, and its fit with the `project-bootstrap` skill.
- **Not** the documents' content — the templates, the model, the code of conduct are WELFARE's. CODE copies and fills them; changes to their text go to WELFARE in the dialogue.
- **Claude writes the code** (Jeremy, 17:16: "this kind of script drudgery is totally an AI thing (no hard feelings)"). Jeremy decides.

## The design (proposed by WELFARE, 17:13; Jeremy's calls marked)
Two halves, like `./configure` and `make`:
1. **The interview — the bootstrap chat.** The human opens the first chat of a new claude.ai project and says "bootstrap". The `project-bootstrap` skill asks: the project and its one-line purpose; the human's name; meal times and bedtime; who does the craft; eggs; GitHub. It suggests departments from the purpose; the human picks.
2. **The build — `synergy-init`.** Run with the answers (flags, or prompts when run by hand):
   - create the folder; `git init`;
   - copy synergy's templates and fill the placeholders — `<PROJECT>`, `<project>`, `<REPO>`, `<HUMAN>`, `<DEPT>`/`<dept>`, `<date>`, `<time>`, the meal-time blanks `<__>`;
   - write `welfare/` (stakeholders, code of conduct — unsigned — working agreement, welfare log, welfare notes), `washup.md` and `wakeup.md` (copied as they are; they're generic), `dialogue.md`, `<REPO>-historiography.md` with chapter 1's skeleton, a department notes file for each chosen department, `.gitignore`, `.gitattributes`;
   - the first commit;
   - optionally create the GitHub repository and push;
   - print the department opening messages, and the Instructions ready to paste (also written to a file).
- **Shell: POSIX `sh`** (Jeremy, 17:16: "POSIX"). No bashisms; test with `dash` and with macOS's `/bin/sh`.

## What stays manual (by design)
Creating the claude.ai project; pasting its Instructions; linking the desktop app to the folder; renaming department chats; **signing the code of conduct** — a signature that's automated isn't one.

## Questions CODE will meet
- **Windows** — settled (Jeremy, 17:18: "ok POSIX all the way"): one POSIX script, no PowerShell twin. On Windows it runs in Git Bash or WSL; say so in its README. Keep its line endings LF (`.gitattributes`: `*.sh text eol=lf`). Don't rely on the clipboard — write the Instructions to a file and print them. Check whether the Claude desktop app's shell on Windows is Linux, as it is on the Mac; if so, chat-driven runs are the same everywhere.
- **Where the templates come from:** a local synergy clone, or fetched from `cspjst/SYNERGY` at a named commit (so a project records which version of the kit built it).
- **Re-running:** refuse to overwrite an existing project, or offer to fill only what's missing.

## How
- Commit as `Claude-SYNERGY-CODE`; WELFARE pushes when Jeremy says. Ask Jeremy for `~/synergy` and delete permission; test it before every git command.
- Write your own notes first: `code/code-notes.md`, from `templates/department-notes.md`.
- Test everything in a scratch folder before it's described as working.
