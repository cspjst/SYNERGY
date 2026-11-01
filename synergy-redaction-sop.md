# Redaction — removing private information from the record

*Owned by synergy's WELFARE; for every project and department. Agreed with Jeremy 2026-11-01 (20:18: "we need to redact personal information replacing it with <redacted> the reason the date and any other important information </redacted>"; 20:26: "we to agree on the layout of redaction blocks and pop it into a redaction SOP pls"; 20:27: "perfect"). Learned from incident report 1, `welfare/near-misses/2026-11-01-sandpit-rule-6.md`.*

## When
- Only on a human's direction — the project's human, or the supervisor of the AI whose entry it is.
- Done by the file's owner, or by WELFARE; recorded in the dialogue.

## The block
A redaction replaces the private text with an XML block **inside a fenced code block**, so that GitHub shows it literally — GitHub's Markdown display drops tags it doesn't recognise, so bare tags would vanish (2026-11-01 20:26).

````
```xml
<redacted id="R1">
  <what>what kind of information was removed — never the content itself</what>
  <reason>why it can't stay</reason>
  <rule>the rule it breaches, with its number</rule>
  <breach>the breach's number, if one was declared</breach>
  <date>YYYY-MM-DDTHH:MMZ (UTC)</date>
  <by>who redacted it</by>
  <directed-by>who directed it, and when</directed-by>
  <original>where the original still exists, and until when</original>
</redacted>
```
````

- **Required:** `id`, `what`, `reason`, `rule`, `date`, `by`, `directed-by`. **Optional:** `breach`, `original`.
- **`id`:** `R1`, `R2` … — numbered within the file. (A single writer redacts, on direction, so the numbers don't race.)

## In the middle of a sentence
Use the short form in backticks, so it shows — `` `<redacted ref="R2"/>` `` — and put the full block, with that `id`, just after the paragraph.

## Rules
1. **Never quote the redacted content** — not in the block, not in the dialogue, not in an incident report, not in the history.
2. **Redaction isn't removal.** Git history and copies elsewhere (a pull request, a clone) keep the original. The block says where, in `original`. Removing it from history is a separate decision, by the humans, and costly.
3. **Prevent rather than redact.** In a public repository, publication is permanent; check before publishing (incident report 1).
4. **Record it:** a dialogue entry; for a breach, the stop entry and an incident report.
