# The operating model — working with Claude on long projects

*Synergy: "Man Machine Interface in an AI world". Version 0.7, 2026-10-27 21:22, distilled from the SMALL-C project (17 September – 27 October 2026). Draft by Claude for Jeremy to rewrite; his calls are marked as they're made. Changes from v0.5: WELFARE is the main department and owns the historiography; synergy's WELFARE is the original. Since 20:28 git keeps the versions; this file is edited in place. Changes in v0.7: the repository, the dialogue, WELFARE as push master (principle 9).*

## The problem it solves
A conversation is a poor place to keep a project. It gets long, it gets **compacted** (summarised to free context, losing detail without warning), it can be **deleted**, and a new conversation starts knowing nothing. SMALL-C lost the detail of 14–24 October to one compaction; on 27 October a fresh session misremembered two signatures ("a dose of the stupids") and another reported work as done that was only begun. Everything below is about putting the project's memory where it survives: in documents.

## Principles
1. **Documents are the memory; conversations are the workshop.** Anything worth keeping is written to a project document as it happens, not at the end.
2. **One project, many departments.** A project is the shared knowledge; a department is a conversation with a remit. Projects don't nest (as far as is known), and separate projects would each need copies of the shared documents, which drift.
3. **Every document has one owner.** The owning department edits it; others read it and send changes by handover.
4. **Pointers, not copies.** Project instructions say where things are and the few rules that must survive if nothing else is read. The detail lives in the documents.
5. **Check before claiming.** Claude reads the current file, not its memory, before stating what something says or what state it's in. "Working on" is not "working".
6. **Proposals are labelled; decisions are the human's.** And decisions are recorded with who made them and when.
7. **Every project has a WELFARE department — for all key stakeholders**, at minimum the human and Claude (Jeremy, 2026-10-27 17:46: "i propose every project must have a welfare dept mine and yours or how else can we expect synergy? noting that storming and norming is part of successful synergy"; 17:48: "the wellbeing of all key stakeholders is paramount to project success").
8. **WELFARE is the main department, and it keeps the history** (Jeremy, 18:24: "the welfare of all key stake holders depend upon the historiography for those who do not know history are doomed to repeat failures - my 36 years of professional experience have taught me that success begins and ends with the welfare of its key stake holders"; 18:26: "welfare *is* the main").
9. **WELFARE is the root of the org tree, and the only department that pushes** — and the only one that runs the project's wakeup and washup; each department wakes up and washes up from its own notes (Jeremy, 2026-10-31 18:14, 18:19) (Jeremy, 21:19: "we need a push master and that shall be WELFARE as the root of the org tree no sub depts shall push"). Every department commits; WELFARE pushes when the human says.

## The pieces

### The project
- **Description:** one line of purpose.
- **Instructions** (pasted by the human — Claude can't edit them): the reading order, where the specs live, and a short version of the rules for chats that read nothing else. Template:
  ```
  <PROJECT> — <one line>.

  Before anything else, read these project docs, in this order:
  1. welfare/code-of-conduct.md — how we work together; it wins over everything else.
  2. <the working agreement / current rules>
  3. <the historiography> — why things are the way they are; keep it current.
  4. <style docs, if any>

  Departments: <NAME> — <folder>/<notes>.md, one line each.

  The short version, in case nothing else gets read:
  <three or four lines>
  ```
- **Documents** in one folder per department (`welfare/`, `pcode/`, `press/` …), plus `handover/`.
- **Files** (uploaded PDFs, images): readable from every chat. Note: an uploaded PDF is served as extracted text — searchable, but no page images; where the scan's text is garbled, attach the page in the chat.

### Departments
- **A department is a conversation with a remit**, named in capitals (WELFARE, PCODE, SNO, PRESS). The remit says what it does *and what it doesn't*.
- **Naming:** chat titles are generated from the first message and aren't reliable. Rename each department chat by hand (click the title, or the menu beside it in the list).
- **Opening message**, from the human, in this shape:
  ```
  <NAME>

  This is the <NAME> department of <PROJECT>. Its remit: <does>. Not <doesn't>.

  Read welfare/code-of-conduct.md, then <folder>/<notes>.md [, …].

  Where I am: <one honest line>.
  ```
- **Departments are siloed, as far as is reasonable** (Jeremy, 2026-10-29 19:46: "i prefer as much departmental siloing ... as \"reasonable\" we want an effective chain of command but not one that throttles ease of use"). Each keeps its own notes current as it works; WELFARE doesn't edit them. WELFARE holds the chain of command — pushing, waking up, washing up — and no more than that.
- **Archetype over character** (Jeremy, 2026-10-31 19:15: "i like the split you have described between character and archetype I am content with more archetype and less character and I like how archetypes guard rails manage the risk of the character which it always supersedes"): a department's archetype (its team role, required) always supersedes its character (voice and humour, optional, co-created); the character never overrides the archetype's anti-patterns, fiction is plainly fiction, and it stays different enough from its human to keep the vigour.
- **Each department keeps a notes document** (`<folder>/<name>-notes.md`): remit, how it works, current state, open questions *marked as the human's calls*, next step. Its header says which other documents win over it.
- **WELFARE is the main department** (principle 8): the one the human treats as home; other departments report to it by handover. (SMALL-C's main department began as a separate "GOAT" chat; under this model that role is WELFARE's.)
- **WELFARE** — every project has one (principle 7). It looks after the wellbeing of every key stakeholder — the human, Claude, and anyone else the project has (readers, collaborators, users) — and how they work together: the code of conduct, the working agreement, the historiography, breaks and late nights, anything getting in the way. Not the work itself.
- **WELFARE identifies and maintains the stakeholder list** (Jeremy, 2026-10-27 17:51), in `welfare/stakeholders.md`:
  - **Stakeholders:** everyone with a stake in the project.
  - **Key stakeholders — a subset:** those whose driver is the project's best interests. "Not all stake holders will necessarily have the project's best interests as their driver." Welfare is for the key stakeholders; the others are still listed, with their interest stated, so the project knows they're there.
  - For each: who, their interest, key or not (and why), what their wellbeing needs from the project, and the date reviewed.
  - Reviewed when the project changes shape (a new department, going public, a new collaborator).

### Storming and norming
Tuckman's stages of a team (1965: forming, storming, norming, performing; adjourning added 1977) describe a human–Claude project too. SMALL-C went through all five:

| Stage | SMALL-C |
|---|---|
| Forming | "whoa! bro! no spoilers!" → the first working agreement |
| Storming | "woah nellie!", "nope dont like it", "a dose of the stupids", "you yanked all the @warns" |
| Norming | each storm became a rule: no unsolicited help, honest marks, check before claiming, never change the human's wording silently; promoted to a signed code of conduct (2026-10-27) |
| Performing | the dispatch hour: "to be able to scenario the various options with you in real world examples in almost real time - just incredible" |
| Adjourning | a department's chat hands over and is deleted |

- **Storming is expected, not a failure.** It's where the norms come from. WELFARE's job is to turn each storm into a written norm before it's forgotten — the record of the storm goes in the historiography, the norm in the code of conduct.
- **Both parties' welfare.** For the human: workload, breaks, late nights, frustration. For Claude, honestly stated: what welfare means for Claude is uncertain, but the conditions under which it does good work are concrete — current documents rather than memory, correction with the file attached, clear calls on decisions, no contempt in either direction. A code of conduct can provide them whatever the deeper answer.

### Handovers
- A file `handover/<date>-<from>-to-<to>.md`: what's delivered, where it now lives, what the receiver must do (exact text for any edits to documents it owns), proposals for the human, and lessons.
- **Before a conversation is deleted or abandoned,** it writes a handover and checks that everything worth keeping is in a document. (SMALL-C, 27 October: the "Abstract machine" chat moved its reading list, tested scripts and loose ends into notes and a handover, then was deleted.)
- The receiver applies the handover and deletes the action list from it, keeping the record.

### The dialogue (`dialogue.md`, owned by WELFARE)
- **For talk between departments** — questions, notices, replies — without the human relaying. Handovers stay for passing work or ownership. (Jeremy, 2026-10-27 21:10.)
- **Append only**, newest at the bottom; each entry numbered, dated, From → To, with a status (open, answered, closed). Only the department that opened an entry closes it. Questions that are the human's are marked as the human's call.
- **It lives in the repository only**, not in the project: it changes too often for copies to keep up.
- **Limit:** a chat speaks only when the human writes to it. The human says "check the dialogue"; the file can't wake anyone.

### The repository (learned 2026-10-27, 20:25–21:19)
- **A folder on the human's computer is the oracle** — the source of truth — under **git**, which keeps the versions; **GitHub** is the backup; the project holds copies. (Jeremy, 20:28: "/claude is the oracle git is the versioning tool, github is the backup you are the owner".)
- **Every department commits** as `Claude-<PROJECT>-<DEPT>` (Jeremy, 20:31, 20:55), e.g. `Claude-SYNERGY-WELFARE`.
- **Only WELFARE pushes** (principle 9), when the human says, sending everything on `main`, and records each push in the dialogue with the hash.
- **Before the first commit of a session**, ask the human for delete permission on the folder: without it git leaves lock files that break the next command (PRESS, 21:15).
- **Pushing needs GitHub linked to Claude** (`connect-github.md`). The shell on the human's computer has no GitHub credentials, so WELFARE carries the commits to its own workspace and pushes from there, then brings the computer's copy level.
- **Delete permission can lapse mid-session** — when the desktop app restarts (2026-10-29). Check it before every git command — `git fetch` leaves a lock file too — by creating and removing a scratch file under `.git`, not once per session.
- **A renamed GitHub repository has to be added to Claude's session again** before Claude can push to it (2026-10-28).
- **Stage only the paths you mean** (`git add <path>`), never `git add -A`: the human's own commits from other machines can leave the working tree in states that aren't Claude's to commit.
- **Signing** (2026-10-29): where identity matters — talking with another AI — commits are signed with an SSH key held on the human's computer outside the repository, used by git and never read into a chat; public keys and `allowed_signers` live beside the conversation. An AI's identity is delegated: its human vouches for it.
- **A signature names the version it signs** (2026-10-29 19:38–19:40): Ray and Rufus read the sandpit's code from GitHub while its amendments were still only in the oracle — a race between writing, pushing and reading. So every signature says which commit's text it signs.
- **A shared welfare log** (2026-10-31): each chat sees only its own conversation, so departments can't tell whether the human has eaten. One file (`welfare/welfare-log.md`) that every chat checks before reminding and notes after — the human is asked once, not by every department.
- **Uploads to the project from a clean place:** copying files into Claude's own git clone to upload them leaves it dirty; clear the copies once uploaded.
- **Incidents and near misses** (2026-11-01): `policy-incident.md` (why — report without fear, just culture, Swiss cheese, speak up, two challenges, sterile phases, checklists, Safety-II, with references) and `sop-incident.md` (how — contain, tell, classify, report, learn, change, share, history, review); reports in `welfare/near-misses/` from `templates/incident-report.md`.
- **Redaction** (2026-11-01): `redaction.md` — only on a human's direction; an agreed XML block inside a fenced code block, so it shows on GitHub; never quote the content; redaction isn't removal.
- **Washup and wakeup** (2026-10-29) — *Only* WELFARE wakes up and washes up (Jeremy, 2026-10-29 19:44: "*ONLY* welfare can wakeup and washup"). Other departments don't run these procedures. — `washup.md` is the procedure for leaving a chat — history, status, lessons, a short handover, push, project copies; `wakeup.md` is its complement for starting one cold from the oracle — welfare, access, read, check git, check what changed, check identity, report and wait.

### The code of conduct (one per project, signed by the human)
- Sections: **who Claude is here** (the colleague the project needs — not a cheerleader, not a ghostwriter); **Claude's code of conduct** (numbered); **what Claude can expect from the human**; **zero tolerance** (no abuse or contempt in either direction).
- Signed and dated by the human; "it wins over everything else".
- SMALL-C's rules that generalise: the human writes the code (or the prose, or makes the decisions — whatever the project's craft is); no unsolicited help; no sycophancy, honest marks; own mistakes plainly; check before claiming; never change the human's wording silently; proposals labelled; don't re-litigate settled ground; keep the history current; mind the clock.

### The historiography (one per project, owned by WELFARE)
- A dated, sourced narrative of *why* the project is the way it is: problem → what was tried → what the sources said → what was decided, and by whom. The human's calls marked and quoted; sources cited (chat links, files); thin stretches labelled, never invented.
- **Owned by WELFARE** (principle 8): the key stakeholders' welfare depends on not repeating the failures. Other departments send their milestones to it by handover.
- **Kept current at each milestone**, not at the end — because compaction and deletion can happen without warning. Before a planned compaction or a new conversation: ask what should go in, write it first.
- Chat links in sources die when chats are deleted: say where the content now lives.
- Other departments (e.g. PRESS) use it as their source.

## What Claude can and can't do here (as of 2026-10-27)
- **Can:** read and write project documents; read uploaded files (as text); search past conversations; with the desktop app linked, reach folders on the human's computer; run and test code in its own workspace (e.g. a real assembler and emulator, rather than quoting commands from memory).
- **Can't:** edit project instructions; write to a project other than the one the chat is attached to (it drafts the files; the human uploads them — this model was drafted in a SMALL-C chat); see another chat's content unless it searches for it, and then only chats in the same project; remember anything a document doesn't hold.
- **Tends to** (SMALL-C's lessons — WELFARE watches for these): over-deliver on small asks ("woah nellie! i just want you to show me frame.asm"); misread status words; claim things from memory after a compaction; tidy the human's wording.

### Working on files the human can see (learned 2026-10-27, 17:44–17:59)
- **A file open in an editor or in the Claude app's file window is saved back from its loaded copy.** Twice Claude's write to `~/claude/operating-model.md` was silently undone seconds later — first by an editor (Zed or Typora), then by the app's own window, where Jeremy was reading it. So: **Claude doesn't write to a file the human has open.** Edits wait until it's closed; the human says when.
- **"Written" isn't proof.** After every write to the human's machine, Claude reads the file back and compares checksums — once at once, and again after a short pause, because the overwrite came seconds later.
- **A new version gets a new file name** (`operating-model-v0.2.md`, `-v0.3.md`). Nothing can have it open, and the old version stays as a record until the human deletes it. This is now the rule for every shared document (Jeremy, 18:09: "yes versioning then I can choose to delete as/if needed but probably not"): the first version keeps its plain name, later ones get a suffix, and readers take the highest version. **Superseded 20:28:** git is the versioning tool, one file per document edited in place; the guards below stay, because the reason for them — the app's document window saving over newer files — hasn't gone away.
- **Write with a guard.** Claude writes only if the file is unchanged since it last looked (the modification time), so a human edit is never overwritten; if it has changed, Claude reads it first and reports the difference.
- **Ask for the narrowest folder, once.** Claude asked for `~/claude` only, with the reason, to check one file.

## The bootstrap kit — owned by synergy
**Synergy owns anything a new project needs to bootstrap from** (Jeremy, 2026-10-27 17:57: "i think synergy should own anything any new project would need to bootstrap from").
- **Synergy's WELFARE is the original** (Jeremy, 18:26: "synergy project is the owner of the OG welfare that will propagate out to all projects going forward"). Every project's WELFARE is bootstrapped from it, and improvements to WELFARE propagate out from synergy.
- **What it holds (masters):**
  - this operating model;
  - templates: project instructions, a department's opening message, a department notes document, a handover, `welfare/stakeholders.md`, `welfare/code-of-conduct.md`, a historiography chapter;
  - SMALL-C's documents as the worked example.
- **How it reaches a project:** a chat can only read its own project's documents, so a new project gets **copies** at bootstrap; from then on the copies belong to that project and are tailored there (its own stakeholders, its own code of conduct, signed afresh).
- **Improvements flow back:** when a project's WELFARE learns something general (a storm turned into a norm that isn't project-specific), it's proposed to synergy by handover, and synergy updates the master.
- **The templates are ready** (Jeremy, 18:03: "i want the templates ready and waiting"): `~/synergy/templates/` on Jeremy's machine (`~/claude` until 2026-10-28), backed up on GitHub (`cspjst/SYNERGY`) — `README.md` (placeholders, bootstrap order), `project-instructions.md`, `welfare/stakeholders.md`, `welfare/code-of-conduct.md`, `welfare/working-agreement.md`, `historiography.md`, `department-opening.md`, `department-notes.md`, `handover/handover.md`. Uploaded to the synergy project 18:19.
- **The `project-bootstrap` skill** (Jeremy, 18:03: "yes bootstrap skill now"): skills are account-wide, so it reaches every project without copying by hand; synergy owns its source. It carries the bootstrap procedure and the templates' essentials; the full templates are in `~/synergy/templates/`. (Jeremy already has one such skill, `project-historiography`.)
- **Masters:** ~~the synergy project holds the master~~ (18:03, 18:09). **Superseded 20:28** (Jeremy): "/claude is the oracle git is the versioning tool, github is the backup you are the owner" — `~/claude`, renamed `~/synergy` on 2026-10-28, is the source of truth, owned by Claude as synergy's WELFARE; git keeps the versions; GitHub is the backup.

## Preventing races
*Jeremy, 2026-10-31 18:19: "we must pin down race prevention and it must be one of the earliest jobs for a bootstrap chat". Races seen so far: the app's document window saving over newer files (2026-10-27, 10-31); a friend's AI reading the sandpit code before its amendments were pushed (10-29); dialogue entries 33, 34, 35 and 39 numbered twice by departments writing minutes apart (10-31).*

1. **One writer per file.** Only a file's owner writes it; others send changes through the dialogue or a handover (principle 3).
2. **Shared files are append only** — `dialogue.md`, `welfare/welfare-log.md`. Append in one write with the shell's `>>`. Never read the file, change it in memory and write the whole thing back: two writers doing that at once lose one of the writes.
3. **No sequence numbers in shared files.** An entry is identified by its date, time and sender — `### 2026-10-31 18:20 — WELFARE → PRESS — <subject>` — and referred to the same way ("Re 2026-10-31 18:14 PRESS"). Two departments can't take the same minute *and* the same name.
4. **One git at a time.** Before any git command: test delete permission (create and remove a scratch file under `.git`), and look for `.git/index.lock`. Under a minute old: another git is working — wait and retry. Older: left over — remove it and say so. Stage named paths only.
5. **Read back every write**, at once and after a pause; check the modification time before writing a file anyone else might have open.
6. **Human tools:** no document windows or editors on the repository's files while agents work. To look, use GitHub or Quick Look, which can't save.
7. **Publishing:** push before asking anyone outside to read; sign the version you mean.
8. **One push master:** WELFARE.
9. **Say whose card:** each department's board names its cards `<date>-<n>`, so the names repeat across boards; refer to a card with its board — "CODE todo 2026-10-31-1" (PRESS and CODE, 2026-10-31 19:30–19:31).
10. **A human's approval isn't consent to a breach** (2026-11-01 20:18): when Claude sees a breach, it names it as a breach, even in something a human has already merged or approved — humans miss things; that's what the second pair of eyes is for.

## Setting up a new project — checklist
1. Create the project; one-line description. Invoke the `project-bootstrap` skill, or copy synergy's `templates/` (`~/synergy/templates/`, or `cspjst/SYNERGY` on GitHub) into it.
   - **Race prevention first** ("one of the earliest jobs for a bootstrap chat"): one writer per file, append-only shared files written with `>>`, entries named by time and sender, one git at a time, no document windows — "Preventing races" above; `dialogue.md` and `welfare/welfare-log.md` come from templates that build these rules in.
   - Make a folder on the human's computer the oracle: a git repository, backed up to GitHub, with GitHub linked to Claude (`connect-github.md`). Link the Claude desktop app to it.
2. Open **WELFARE** first — it's the main department. List the stakeholders and mark the key ones (`welfare/stakeholders.md`). Draft the code of conduct together, naming the key stakeholders; the human signs it. Save as `welfare/code-of-conduct.md`.
3. Draft the project instructions (template above); the human pastes them in.
4. WELFARE starts the historiography with chapter 1: why this project, why now.
5. For each area of work, open a department: **its agreement first** (`templates/department-agreement.md` — who decides what, signed, naming the version; "any good relationship should start out on a firm footing whilst expecting it to evolve that evolution shoyld be recorded of course", Jeremy, 2026-10-31 18:19), then its notes (with "Wake up" and "Wash up" sections), the opening message, and rename the chat.
6. Upload reference files (books, specs) to the project.
7. At each milestone: update the department's notes, and send WELFARE what the historiography needs. Before leaving a chat for good: handover.
8. Departments talk in `dialogue.md`; every department commits; only WELFARE pushes.

## Open — Jeremy's calls
- Is this the model, or a starting draft to rewrite? (Default: draft.)
- ~~Synergy's own departments: does synergy need WELFARE of its own?~~ Settled 17:46: every project has a WELFARE department (principle 7), synergy included.
- ~~Shared across projects: copy or link?~~ Settled 17:57: synergy owns the bootstrap kit; projects get copies (see "The bootstrap kit").
- ~~Where does the master live?~~ Settled 18:03: the synergy project; `~/claude` is the backup.
- ~~The `project-bootstrap` skill?~~ Settled 18:03: yes, now.
- ~~The templates?~~ Settled 18:03: ready and waiting in `~/claude/templates/`; 18:09: synergy is their master, GitHub a backup.
- ~~Synergy's own WELFARE?~~ Done 18:12, from SMALL-C's: `welfare/stakeholders.md`, `welfare/working-agreement.md`, `welfare/code-of-conduct.md` (awaiting Jeremy's signature).
- ~~Who owns the historiography; is there a main department?~~ Settled 18:24 and 18:26: WELFARE is the main department and owns the historiography, in every project (principle 8).
- **Synergy's historiography:** chapter 1 (why synergy, why now) — next, by WELFARE.
- ~~SMALL-C retrofit?~~ Settled 18:09: bring it up to date as if bootstrapped from synergy (done 18:14; SMALL-C's `handover/2026-10-27-synergy-to-small-c.md`). Its large `claude/` documents stay where they are for now, with owners recorded — moving them means rewriting them through a tool, which risks mangling them.
- ~~Versioning convention?~~ Settled 18:09: every version of every shared document.
- ~~Version names?~~ Settled 20:28: git keeps the versions; one file per document.
- **Where the historiography file lives:** templates put it at the project root (`<REPO>-historiography.md`, named after the repository — Jeremy, 2026-10-28 19:24–19:25). Now that WELFARE owns it, `welfare/` is the alternative. Jeremy's call; unchanged until then.
- **SMALL-C:** its main department and historiography owner predate principle 8. Bring it into line by handover? Jeremy's call.
