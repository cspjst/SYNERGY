# tools

Small POSIX `sh` tools for synergy, written by Claude-SYNERGY-CODE at Jeremy's direction (`code/code-agreement.md`). They run on macOS, Linux, and on Windows in Git Bash or WSL. Covered by the repository's licence.

## `tools/board` — the boards in a browser
```
tools/board
open synergy-board.html
```
Reads every department's board (`<dept>/<dept>-todo.md`; `templates/` is skipped) and writes one self-contained page, `<repo>-board.html`, at the top of the repository: each department's two boards side by side, every card's number, title, status, category and estimate, and the human's Next and Doing totals across all boards against their limits (3 and 2), red when over. Works from anywhere in the repository.

- **Read-only:** it never writes a board. The Markdown boards are the truth; the page is a snapshot, rebuilt each run.
- **Kept out of git:** the page is derived, so it isn't committed (for now via `.git/info/exclude`, on this machine only).
- **Nothing fetched:** no server, no scripts or fonts from the web.
- **Reads** the signed format (`synergy-kanban-policy.md`) and the old one of 2026-10-31.
- `tools/board -h` for usage. Exit status: 0 done; 1 not in a repository, or no boards; 2 a bad argument.

## `tools/board-test` — its tests
```
sh tools/board-test                                  # under sh
tools/board-test dash "bash --posix" "busybox sh"    # under several shells
AWK=mawk tools/board-test                            # with another awk
```
Builds a scratch repository from copies of the real boards, plus a board in the old format, an empty board, a template and a hostile card; runs the tool; and checks the page: every card shown, the totals, escaping, the template and fenced examples skipped, the boards unchanged, and the exit statuses. Never touches the real boards.
