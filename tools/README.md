# tools

Small POSIX `sh` tools for synergy, written by Claude-SYNERGY-CODE at Jeremy's direction (`code/code-agreement.md`). Tested on macOS and Linux; written for Windows in Git Bash or WSL too, but not yet tried there. Covered by the repository's licence.

## `tools/board` — the boards in a browser
```
tools/board
open synergy-board.html
```
Reads every department's board (`<dept>/<dept>-todo.md`; `templates/` is skipped) and writes one self-contained page, `<repo>-board.html`, at the top of the repository. Works from anywhere in the repository.

- **Your board, first:** everything the human owes — every department's Waiting for you, Next and Doing — merged into one board, each card named with its department.
- **Then each department:** its two boards side by side, card numbers without the department prefix.
- **On every card:** number, title, status, estimate, and its category as a coloured pill — Decide, Do, Read.
- **Colour, accessibly** (WCAG 2.2): each department has a stripe, from its name, so it stays the same as departments are added; colour is never the only signal — the department's name and the category's word are always written beside it (1.4.1); text contrast is 4.5:1 or more in light and dark (1.4.3), stripes 3:1 or more (1.4.11), checked with the WCAG formula, not by eye.
- **The human's load:** Next and Doing totals across all boards against their limits (3 and 2), red when over.

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
Builds a scratch repository from copies of the real boards, plus a board in the old format, an empty board, a template and a hostile card; runs the tool; and checks the page: every card shown, your board on top, the totals, the pills and colours, short numbers, escaping, the template and fenced examples skipped, the boards unchanged, and the exit statuses. Never touches the real boards.

## Keeping a version
Don't copy or rename a file to keep it — git already keeps every version. Mark the one you want with a tag:
```
git tag -a tools-board-v1 342d066 -m "why it's worth keeping"   # mark it
git push origin tools-board-v1                                   # back it up (WELFARE pushes, on Jeremy's word)
git show tools-board-v1:tools/board                              # read it
git diff tools-board-v1 -- tools/board                           # see what's changed since
git checkout tools-board-v1 -- tools/board                       # bring it back (overwrites the working copy)
```
The file keeps its one name, so everything that uses it — tests, other tools, links — still finds it. (Jeremy, 2026-11-03 18:25, after renaming the tools to `_1` to keep them: "should have done that through instead of 'helping'".)

**Tags so far:** `tools-board-v1` — `tools/board` as Jeremy accepted it on 2026-11-02 22:34 ("a good first version simple and does the job"), on commit `342d066`. That commit's `tools/board-test` has the hang fixed later in `6ae7d5b`; use the current test.
