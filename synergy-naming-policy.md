# Naming — policy

*Owned by synergy's WELFARE; for every project. How files and folders are named, and why. The procedure is `synergy-naming-sop.md`. Agreed with Jeremy 2026-11-01: 20:39, "yes we also need a policy-naming and sop-naming :D shall we figure out our file naming policy what can we learn from whats already out there as policies must be evidence based"; 20:49, "1. whatever the research recommends 2. all lower as per research 3. yes"; and the one exception, "with one exception to enable travelling files pls keep folder names". This file is named by its own rules. Updated 2026-11-01 21:40 with rules for **words** as well as files (Jeremy, 2026-11-01 21:28: "thats another CS naming legacy that falls foul of ethics such as the infamous master-slave pattern ... is there any precedent out there for how to handle CS naming that has aged like milk?"; 21:35: "pls update the naming policy with this new information").*

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

## Words, as well as files
*Names live in prose too — headings, rules, card titles. Some technical terms have aged badly; others are just unclear. How synergy handles them follows the industry's precedents: the Inclusive Naming Initiative's tiers (2021), the Linux kernel's coding style (5.8, 2020), NIST IR 8366 (2021), and the IETF's 2021 statement on inclusive language.*

11. **Prefer the plain word.** Choose the term that says what happens to the work, so a newcomer can't misread it — "collision", not "race condition" (Huffman, 1954, gave "race" its sense of signals racing; it's on no inclusive-language list, but "collision" is clearer).
12. **Check new terms against the Inclusive Naming Initiative's word lists** before adopting them. **Tier 1** ("replace immediately" — e.g. *master*, *master-slave*, *whitelist*, *blackhat-whitehat*, *abort*, *cripple*): never in new work; replaced in living documents. **Tier 2** ("strongly consider" — *sanity-check*) and **Tier 3** ("consider" — e.g. *man-in-the-middle*, *hallucinate*, *segregate*): replaced where a clearer word exists. **No change** (e.g. *blackbox*, *red team*, *parent child*): kept. The lists change; check the current one, and record the date checked.
13. **Weigh each term:** the harm it may do; how clear it is; the alternatives; and the cost of changing it. Record the decision and its reason, with the human's words, in the working agreement — "no change" included, as the Initiative publishes its own.
14. **Replace in living documents; never in quotes or dated records.** A human's words are never changed (code of conduct, rule 5); the history, handovers, the dialogue's past entries and settled decisions keep the words they were written with. As the Linux kernel does, an established interface may keep an old term where changing it would break things — and says why.
15. **Keep the old term as an alias,** once, where the new term is defined — "collisions (formerly 'races')" — so that searches for the old word still find the new.

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
- Inclusive Naming Initiative. *Word lists*, v1.0 (tiers 1–3 and "no change"; checked 2026-11-01). https://inclusivenaming.org/word-lists/inclusive-naming-word-lists-v1.0 ; https://inclusivenaming.org/word-lists/no-change
- Linux kernel. *Coding style*, §4: inclusive terminology (from 5.8, 2020). https://lore.kernel.org/ksummit/87o8oh0y4l.fsf@intel.com/T/
- National Institute of Standards and Technology (2021). *Guidance for NIST Staff on Using Inclusive Language in Documentary Standards*, NISTIR 8366.
- IESG (2021). *Statement on inclusive language.* https://datatracker.ietf.org/doc/statement-iesg-iesg-statement-on-inclusive-language-20210511/ ; Knodel, M., & ten Oever, N. *Terminology, power, and inclusive language*, IETF draft. https://datatracker.ietf.org/doc/html/draft-knodel-terminology-05
- Huffman, D. A. (1954). The synthesis of sequential switching circuits. *Journal of the Franklin Institute*, 257(3), 161–190; 257(4), 275–303.
- ISO 9001:2015, clause 7.5, *Documented information* — the control of policies, procedures, forms and records.
