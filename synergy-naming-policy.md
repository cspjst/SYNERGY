# Naming — policy

*Owned by synergy's WELFARE; for every project. How files and folders are named, and why. The procedure is `synergy-naming-sop.md`. Agreed with Jeremy 2026-11-01: 20:39, "yes we also need a policy-naming and sop-naming :D shall we figure out our file naming policy what can we learn from whats already out there as policies must be evidence based"; 20:49, "1. whatever the research recommends 2. all lower as per research 3. yes"; and the one exception, "with one exception to enable travelling files pls keep folder names". This file is named by its own rules.*

## Purpose
Names that sort correctly, work on every operating system, read well to humans and to agents, and still say what a file is when it travels away from its folder.

## Rules
1. **Lowercase only** — files and folders (ISO 9660 practice; Krewer & Wahl). It also avoids two names differing only in case, which macOS and Windows treat as one file and git as two.
2. **Letters, digits and hyphens** in documents (`a`–`z`, `0`–`9`, `-`, and the `.` before an extension). No spaces; none of the characters operating systems reserve — `\ / : * ? " < > |` (Microsoft; the backslash file of 2026-10-29 is synergy's own evidence). Hyphens are the most common recommendation in place of spaces.
3. **Code follows its language:** underscores where identifiers need them — Jeremy's C, e.g. `dos_error_types.h`, `dos_file_services.c` (2026-11-01 20:49: "yes").
4. **Folder name first — the exception, for travelling files.** A file starts with the name of the folder it lives in (singular where natural): `welfare/welfare-notes.md`, `templates/template-todo.md`, `handover/handover-2026-10-31-welfare-to-code.md`. At the top level, the folder is the repository: `synergy-operating-model.md`. Records guidance says not to repeat the folder's name (UCL, rule 3); synergy does, deliberately, because its files travel — into the claude.ai project, into new projects, into chats — and outside its folder `todo.md` could be anything. It's the same reason C programmers prefix every name with its namespace (Jeremy, 20:46: "my brain has decades of over coming C's lack of name spaces with naming conventions!").
5. **Then the subject, then the kind** — the most important element first (UCL, rule 2), and no word of form at the start (UCL, rule 9): `synergy-incident-policy.md`, `synergy-incident-sop.md`, `welfare-incident-log.md`. The kinds, after quality-management document control (policy → procedure → form → record) and the Diátaxis framework (how-to guides):
   - **`-policy`** — what and why, with its evidence;
   - **`-sop`** — how, step by step;
   - **`-guide`** — a how-to for a human (Diátaxis);
   - **`-log`** — a record, appended to;
   - **`-notes`**, **`-todo`**, **`-agreement`** — a department's working documents;
   - **`template-`** files live in `templates/`; the file each becomes drops the `template-` and takes its new folder's name.
6. **Dates in ISO 8601, `YYYY-MM-DD`,** right after the folder name, for records made in sequence — handovers, incident reports, posts — so they sort by date (ISO 8601; the most-used date standard in Krewer & Wahl's survey).
7. **Numbers with leading zeros** where files are numbered, so 10 sorts after 9.
8. **No versions in names** — git keeps them. (Records guidance adds `_v02`; synergy needn't.) Comparison drafts carry `-v2` only while they're being compared.
9. **Short, but understandable** (UCL, rule 1). Human- and machine-readable; never a random system-generated name (Krewer & Wahl).
10. **Exceptions — conventional names that tools look for:** `README.md` (GitHub shows it), `LICENSE`, `.gitignore`, `.gitattributes`, and git's `allowed_signers`.

## References
- Krewer, D., & Wahl, M. File naming conventions: a literature review and survey of 398 library and archives professionals. *Code4Lib Journal.* https://journal.code4lib.org/articles/13438
- UCL Records Office. *Naming conventions for electronic records.* https://www.ucl.ac.uk/library/collections/records-office/naming-conventions-electronic-records
- Queen Mary University of London. *Electronic File Naming Conventions*, v2.1. https://www.qmul.ac.uk/governance-and-legal-services/media/arcs/governance/information-governance/records-management/Electronic-File-Naming-Conventions-v02.1.pdf
- University of Edinburgh. *Records management: naming conventions.* https://data-protection.ed.ac.uk/records-management/practical-guidance/naming-conventions
- Bentley Historical Library, University of Michigan. *Naming directories and files.* https://bentley.umich.edu/records-management/policies-and-guidance/naming-directories-and-files/
- ISO 8601, *Date and time — representations for information interchange.*
- ISO 9660, *Volume and file structure of CDROM for information interchange* — the restricted character set file-naming guides adapt.
- Microsoft. *Naming Files, Paths, and Namespaces* — reserved characters and names in Windows.
- Procida, D. *Diátaxis* — a framework for documentation: tutorials, how-to guides, reference, explanation. https://diataxis.fr ; Canonical's adoption: https://ubuntu.com/blog/diataxis-a-new-foundation-for-canonical-documentation
- ISO 9001:2015, clause 7.5, *Documented information* — the control of policies, procedures, forms and records.
