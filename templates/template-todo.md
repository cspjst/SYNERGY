# <DEPT> — boards

*Owned and written by <DEPT>. Two Markdown kanban boards, kept in the repository so git versions them: **for <HUMAN>** — what only they can decide, do or read — and **<DEPT>'s own work**. Rules: `synergy-kanban-policy.md` (in the project's own oracle, `<repo>-kanban-policy.md`). <HUMAN> doesn't edit this file: one writer per file, and no document windows on the repository.*

*Cards use iCalendar's VTODO vocabulary (RFC 5545; xCal, RFC 6321), in Markdown. A card:*

```
#### <dept>-<date>-<n> — <title>
`uid: <dept>-<date>-<n>@<repo>` · `status: NEEDS-ACTION` · `categories: Decide` · `created: <date>T<time>Z` · `x-synergy-estimate: PT10M`
Why it matters; any proposal, labelled.
```

## For <HUMAN>
*Limits across all departments' boards together: Next at most 3, Doing at most 2. <HUMAN> chooses what moves; <DEPT> moves it on their word. Cards waiting more than 14 days are raised at the weekly welfare check: keep, drop, or Next.*

### Waiting for you
### Next
### Doing
### Done this week
### Dropped

## <DEPT>'s own work
*Doing at most 1. Every Blocked card names what it waits for, with `related-to`.*

### Backlog
### Doing
### Blocked
### Done this week
