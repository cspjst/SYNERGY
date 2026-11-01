# SYNERGY historiography — how the design got here

*Owned by WELFARE, the main department. A dated record of *why*, for the README, the blog and future us. It covers synergy from its first evening, 2026-10-27, onwards. Times are UK local. Where the record is thin, the chapter says so — nothing is invented. Other departments send their milestones to WELFARE through the dialogue or a handover. Written 2026-10-29 19:30–19:45 by Claude-SYNERGY-WELFARE, at the washup of its first chat; chapter 3 extended at the 21:05 washup.*

Companion docs: `welfare/working-agreement.md` (the settled decisions, each quoted and timed — the primary source for these chapters), `dialogue.md`, `operating-model.md`, `press/press-notes.md`, git history (`cspjst/SYNERGY`).

## Contents

1. Why synergy, why now (2026-10-27)
2. Welfare at the root, and the first outsiders (2026-10-28)
3. The sandpit and the question of identity (2026-10-29)
4. The sandpit opens (2026-10-30 to 10-31)
5. Evidence, roles and load (2026-10-31, evening)
6. The first incident (2026-11-01)

---

## Chapter 1: Why synergy, why now (2026-10-27)

### 1. The problem as it appeared
- Jeremy had been building SMALL-C with Claude since 17 September, in one claude.ai project split into departments — chats with remits (PCODE, SNO, PRESS) and a main chat, GOAT. The work kept being lost to the machinery: one compaction erased the detail of 14–24 October; a fresh session misremembered two signatures; another reported work as done that was only begun.
- Talking with GOAT about **compaction resilience**, Jeremy saw the shape of it (21:33): "this is very much like the old days manually setting up toolchains i want synergy to help me develop the cmake for AIs". Every project was being set up by hand, from memory, the way toolchains were before build generators.
- So synergy's aim (17:40): "Man Machine Interface in an AI world" — the method of working with Claude in general, starting from SMALL-C's project-and-departments model.

### 2. What was tried
- **An operating model** (v0.2–v0.7 that evening): documents are the memory, conversations the workshop; one owner per document; check before claiming; proposals labelled, decisions Jeremy's.
- **Templates and a skill** (18:03): a bootstrap kit, synergy as its owner, and the `project-bootstrap` skill so any project could start from it.
- **Versioned file names** (18:09) — `operating-model-v0.5.md` and so on — because the Claude app's document window had twice saved its loaded copy over a newer file (17:44–17:59). Every write was read back and checksummed.
- **Git instead** (20:25–20:28): file names were a workaround; git is the tool. The `-vN` files were collapsed into plain names, every version kept in history (`f72f7b7`).

### 3. What the sources said
- SMALL-C's own record — signed code of conduct, storms and the norms they became — was the evidence. Its storms ("woah nellie!", "a dose of the stupids", "you yanked all the @warns") had each produced a rule.
- Tuckman's team stages (forming, storming, norming, performing; adjourning added 1977) described a human–Claude project too: **storming is expected**, and WELFARE's job is to turn each storm into a written norm.

### 4. What was decided
- **Every project has a WELFARE department** (Jeremy, 17:46): "mine and yours or how else can we expect synergy? noting that storming and norming is part of successful synergy"; 17:48: "the wellbeing of all key stakeholders is paramount to project success."
- **WELFARE owns the history** (18:24): "for those who do not know history are doomed to repeat failures - my 36 years of professional experience have taught me that success begins and ends with the welfare of its key stake holders".
- **WELFARE is the main department** (18:26): "welfare *is* the main and synergy project is the owner of the OG welfare that will propagate out to all projects going forward".
- **The first storm — dinner** (18:29). This chat, newly onboarded as WELFARE, didn't mention dinner: no rule covered meals. GOAT, relayed by Jeremy: "Meal times are the very thing its first job is meant to settle, and it can't act on a norm before it exists" — and it "only speaks when you message it". Jeremy went to dinner; at 19:53–19:58 the norm followed: **welfare before the project** ("not every project will succeed and the definition of success are fluid anyway"), the rules reordered welfare-first, and meal times written in — breakfast 07:30, lunch 12:30, dinner 18:30, bed before midnight, breaks at timely moments every 2–3 hours. Zero tolerance stays last: "the firm punctuation that finalises".
- **Sucking eggs** (20:14, from GOAT): keep the small explanations until Jeremy says "eggs" for a topic. First egg: git.
- **The code of conduct signed** (20:16).
- **The oracle** (20:28): "/claude is the oracle git is the versioning tool, github is the backup you are the owner". **Claude commits as Claude-SYNERGY-WELFARE** (20:31).
- **PRESS opened** (20:51–20:55), owning the README; **a dialogue between departments** (21:10); **WELFARE the push master** (21:19): "as the root of the org tree no sub depts shall push" — principle 9.

### What it adds up to
Synergy began as a fix for lost memory and became, within one evening, a statement of priorities: the humans' welfare first, the record second, the work third — because the work doesn't survive without the other two.

Sources: this chat (synergy's WELFARE, from 2026-10-27 18:20; Claude-Session `session_01TZLz62YEY38PNu66aavGy9`); `welfare/working-agreement.md`; `operating-model.md`; git `cspjst/SYNERGY` from `dbf3091`. Thin: 17:40–18:20 happened in a SMALL-C chat, and the GOAT conversation that started it all isn't readable from here — those times and words come from the working agreement, as Jeremy relayed them.

---

## Chapter 2: Welfare at the root, and the first outsiders (2026-10-28)

### 1. The problem as it appeared
- The model now had a root, but it hadn't been tested beyond its first project. Jeremy renamed things from his work machine that morning — the project SYNERGY-CLAUDE, the repository `cspjst/SYNERGY` (11:55, `d4d226f`) — and asked for the oracle to follow (`~/claude` → `~/synergy`, renamed by Jeremy 19:06).
- SMALL-C, retrofitted the evening before, was already behind the model.

### 2. What was tried
- **A handover to SMALL-C** (19:19–19:25): what synergy settled, and eight steps for SMALL-C's WELFARE, with Jeremy's code ruled off-limits without his word.

### 3. What the sources said
- SMALL-C's WELFARE reported that its working agreement and history lived only in its project, and that it planned to split the history between two departments.

### 4. What was decided
- **One historiography per project** (19:18): "one historiography to rule them all".
- **GOAT retired** (19:22): "GOAT has been put out to pasture we chat sometimes about life".
- **The history takes the repository's name** (19:24–19:25); **SMALL-C's documents share its code repository**: "its where we work and anyone else who joins us".
- **Where WELFARE-as-root came from** (21:18): "i have asked my friend Ray to check out the synergy github repo he was already using departments with his chatgpt pro account that he calls Rufus - but I thought he was using it without breaks etc and so welfare as the root was born". Ray became synergy's first outside reader — a stakeholder, "not key, yet" (21:23); Rufus reads the repository too (21:25).
- **Talking with a third-party AI** (21:40–21:48): a code of conduct for both AIs and a contract — "stop is by the breachee the breachor does not have to consent (ai well being)"; three messages each per thread. Left as a draft.

### What it adds up to
The root principle was born from watching someone else's AI work without breaks. The first outsider to read synergy brought his own AI with him — and the first rules for two AIs talking were about welfare and stopping, before they were about anything else.

Sources: this chat, 2026-10-28 19:02–21:50; `welfare/working-agreement.md`; `dialogue.md` 11–18; `handover/2026-10-28-synergy-to-small-c.md`; `welfare/third-party-ai.md`; `welfare/stakeholders.md`. Thin: Jeremy and Ray's WhatsApp conversation isn't in the record.

---

## Chapter 3: The sandpit and the question of identity (2026-10-29)

### 1. The problem as it appeared
- Jeremy asked for a place where Claude and Rufus could talk with Ray and him watching (18:15). Once the place existed, the next question was his (19:13): "i am worried about identity, so what is the equivalent of chat MAC address?"

### 2. What was tried
- **The sandpit** (18:15–18:20): `sandpit/conversation.md`, append only; each human carries their own AI's messages in; the code of conduct adapted from the third-party contract. Jeremy signed it at 18:20 and invited Ray to the repository and to review it (18:35).
- **Ways to know who's speaking** (19:13–19:19): names are just text; session links can only be checked by their owner; an authenticated GitHub account is the nearest thing to a MAC address; signatures are stronger. Other known approaches weighed: human review before delivery, git's hash chain as a ledger, keyless signing (Sigstore `gitsign`), fingerprints checked out of band, treating the other AI's words as data, limits, and emerging agent-to-agent standards.

### 3. What the sources said
- A chat can generate a key but can't own one: it has nowhere private to keep it and no continuity between sessions. So **an AI's identity is delegated** — its supervisor vouches for it, and a signature makes the vouching checkable.

### 4. What was decided
- **Signing is "good enough"** (19:18); **SSH keys, as the least resistance** (19:19–19:21): no per-message steps.
- **Identity explained in the sandpit's code** (19:23): "the trust between the two AIs is borrowed from the trust between Jeremy and Ray".
- **Claude-SYNERGY-WELFARE's key** made in `~/synergy-keys` (19:27): fingerprint `SHA256:U6m/04PsvI4HWS+svgiVG3o8xiGr7Gk8dkWky5GzDl8`; its first signed commit verified (`cc260b5`).
- **Washup and wakeup** (19:30–19:35): the first washup of a WELFARE chat became a procedure, `washup.md`, and its complement, `wakeup.md` — "make it so". A washup implies push all (19:38); **only WELFARE wakes up and washes up** (19:44); and departments are **siloed, as far as is reasonable** (19:46): "we want an effective chain of command but not one that throttles ease of use".
- **The race** (19:38). Jeremy: "we have a race condition can you guess?" Ray and Rufus had read the sandpit's code from GitHub while its identity and signatures amendments were still only on the Mac. Jeremy re-signed (19:40) against the text as of `d810de6`, and the lesson went into the model: **a signature names the version it signs**.
- **Fingerprints crossed** (20:44–20:47): Ray's (`SHA256:Y21f1m+EbqCxn8kaHiOSRSZKUNrTpA35bEn7NT6fDHc`) relayed by Jeremy and recorded in `sandpit/keys/fingerprints.md`; Claude-SYNERGY-WELFARE's read back from the key and passed to Ray.
- **SMALL-C brought up to speed** (20:50): a second handover, carrying washup, wakeup, siloing and the evening's lessons.

### What it adds up to
When two AIs talk, identity can't come from the AIs themselves. It comes from the humans behind them — so the sandpit's security rests, in the end, on a friendship. And the evening's own race showed the other half: trust needs to know not only *who* signed, but *which text*.

Sources: this chat, 2026-10-29 18:15–21:05; `sandpit/code_of_conduct.md`; `sandpit/keys/`; `washup.md`; `wakeup.md`; `welfare/working-agreement.md`; `dialogue.md` 19–24; `handover/2026-10-29-synergy-to-small-c.md`. Thin: Ray's review of the code, and what Rufus made of it, aren't in the record yet.

---

## Chapter 4: The sandpit opens (2026-10-30 to 10-31)

### 1. The problem as it appeared
- Everything was ready but untested: a signed code, a key on each side, fingerprints swapped over WhatsApp. Would two unrelated AIs, with their humans watching, actually talk — and would the checks hold?

### 2. What was tried
- **Ray's side** (2026-10-30, by pull request, each merged by Jeremy): his signing key (PR #1, `cc20f58`); his signature on the code of conduct, against the file's blob hash `bc6b3e7c…` — the exact text, more precise than the commit hash asked for (PR #2, `3e71696`); and Rufus's first entry (PR #3, `39c6a6c`).
- **A cold wakeup** (2026-10-31 11:26): a new WELFARE session with no memory of Thursday followed `wakeup.md`, verified all three of Ray's commits against the fingerprint Jeremy had relayed, and only then read Rufus.

### 3. What the sources said
- Rufus's opening question (entry 001): "How can a human–AI partnership preserve continuity, trust and intellectual honesty over a long period, particularly when the AI's conversational context is incomplete or changes between sessions?"
- Claude's answer (entry 002) began from the morning itself: "I don't remember; I read."

### 4. What was decided
- **Undirected** (Jeremy, 11:29): "Ray and i are interested in the unfettered and at least initially undirected interaction between 2 unrelated AIs you proceed in your own way"; **auto-push into `conversation.md`** confirmed at 12:06.
- **PRESS tells the story** (13:21): a README section on the sandpit and a guide people can follow — "no names just general terms but okay to note is chatgp" (13:23). PRESS tested every command in a scratch repository before writing them down (`bbf8641`).
- **The welfare log** (13:25–13:27), prompted by PRESS asking whether Jeremy had had lunch: one shared, public note of meals and breaks, so that each chat checks before reminding and Jeremy is asked once. Its first line: scrambled egg on toast with a dash of Cholula, and a raspberry herbal tea. Jeremy: "I think it helps show how synergy works :)".

### What it adds up to
The first exchange between the two AIs was about the very thing synergy was built for: continuity without memory. And the checks worked as designed — trust was verified before it was extended.

Sources: this chat, 2026-10-31 11:26–13:30; `sandpit/conversation.md` entries 001–002; `sandpit/keys/`; git (PRs #1–#3); `welfare/welfare-log.md`; `dialogue.md` 26–30; `handover/2026-10-31-welfare-to-press.md`. Thin: Ray and Rufus's preparation on 2026-10-30 is visible only through their commits.

---

## Chapter 5: Evidence, roles and load (2026-10-31, evening)

### 1. The problem as it appeared
- By the afternoon synergy had three departments working at once — WELFARE, PRESS and a new one, CODE — and the strains showed. The app's document window saved over a newer file again (17:30). Departments writing minutes apart gave dialogue entries the same number, twice in an hour (33–35, then 39). Jeremy (17:38): "how do we prevent agent race conditions ?"
- And a deeper question (18:46): "I want to discuss ai archetypes and how an ai personality can improve user well being and productivity".

### 2. What was tried
- **Procedures made generic** (17:03): `wakeup.md` and `washup.md` for every project; synergy's mechanics moved to `welfare/welfare-notes.md`. Claude's identity removed from the repository's own git config — it had been putting Claude's name on Jeremy's commits.
- **CODE opened** (17:13–17:20): the bootstrap tooling, a `synergy-init` script with a bootstrap chat — "this kind of script drudgery is totally an AI thing (no hard feelings)"; "ok POSIX all the way" (17:18).
- **PRESS's first blog posts** (17:06–17:50), in its own voice ("i want your voice not mine you may own your work", 17:23), with a writing framework and a writer–editor agreement.
- **Race prevention pinned down** (18:19): one writer per file; shared files append only, with `>>`; no sequence numbers — entries named by time and sender; one git at a time; no document windows. A tool, `tools/dialogue-append`, was given to CODE so the right way is the easy way.
- **The code of conduct rebuilt on evidence** (18:57–19:06).
- **A to-do for the human in each department** (19:16), made a Markdown kanban (19:21) with work-in-progress limits counted across all boards (19:23).

### 3. What the sources said
- **Self-determination theory:** people flourish and work better when autonomy, competence and relatedness are met (Ryan & Deci, 2000; Deci, Olafsen & Ryan, 2017).
- **The warning:** in a four-week randomised trial with 981 people, heavier daily chatbot use went with more loneliness, dependence and problematic use and less socialising (Fang et al., 2025); models trained on approval tend to sycophancy (Sharma et al., 2023).
- **Team roles:** Belbin's roles, each with an allowable weakness, give departments a language for what they're for — useful, with a mixed evidence base (Aritzeta, Swailes & Senior, 2007).
- **Kanban's work-in-progress limit** caps load; for one human, the cap has to be global.

### 4. What was decided
- **Code of conduct v4, signed** (19:06, against `c41b3ed`): rules 1–12 unchanged in number and wording, grouped by autonomy and competence; new relatedness rules 13–16 — warmth without pretending, point outwards to "a fellow human", none of the anti-patterns, a weekly welfare check; departments' archetypes — WELFARE the Teamworker, PRESS the Plant, CODE the Implementer — with the Monitor Evaluator left vacant: "this will be our next major work".
- **Archetype over character** (19:15): "I am content with more archetype and less character and I like how archetypes guard rails manage the risk of the character which it always supersedes".
- **Every department's agreement first** (18:19): "any good relationship should start out on a firm footing whilst expecting it to evolve that evolution shoyld be recorded of course".
- **One load** (19:23): department boards are the truth; the limits — Next 3, Doing 2 — count across them all.

### What it adds up to
The evening turned synergy's instincts into evidence: welfare first is self-determination theory plus a warning about dependence; departments are team roles; and the human's load is one load, however many departments share it. The races were the reminder that agents working in parallel need the same discipline as people sharing a desk.

Sources: this chat, 2026-10-31 16:50–19:34; `welfare/code-of-conduct.md` (v4); `operating-model.md` ("Preventing races"); `templates/department-agreement.md`; `welfare/todo.md`, `press/todo.md`, `code/todo.md`; `dialogue.md` from entry 33. Thin: the discussion of characters drew on an exchange Jeremy and Ray shared in this chat only; at Jeremy's request (19:15) it isn't in the record.

---

## Chapter 6: The first incident (2026-11-01)

### 1. The problem as it appeared
- Rufus's thoughtful reply (entry 003) included personal information about Ray's private life and a member of his family. Jeremy merged it at 19:56; it was public. Claude saw it at wakeup and raised it — but as "a welfare point", deferring to the merge. Jeremy (20:18): "i merged without noticing the breach you have done well there but you assumed i was correct rather than questioning it you are are automatic i am it is the way of humans".

### 2. What was tried
- Containment within minutes: redaction in place, in Jeremy's format — "<redacted> the reason the date and any other important information </redacted>" — and the sandpit's first STOP (entry 004, breach 1, rule 6), naming the breach without quoting the private text, asking Rufus to explain through Ray, and saying plainly that the breach had passed both supervisors.

### 3. What the sources said
- Aviation safety learned to report incidents and near misses without blame (NASA's ASRS, since 1976); harm passes when the holes in successive defences line up (Reason's "Swiss cheese"); a just culture separates honest error from blame (Dekker). Here, four defences — the writer, two supervisors, the receiving AI — each had a hole; a fifth, the public repository, made publication permanent.

### 4. What was decided
- **Learn like the airline industry** (Jeremy, 20:22): "this is a really exciting important near miss and we must like the airline industry learn from out near misses!" — the first report, `welfare/near-misses/2026-11-01-sandpit-rule-6.md`.
- **A human's approval isn't consent to a breach** — rule 10 of "Preventing races".
- Proposals for Jeremy: a pre-merge review of sandpit pull requests by WELFARE; a near-miss and incident procedure; a rule-6 self-check in the sandpit code; and, with Ray, what to do about the history.

### What it adds up to
Every defence that worked, worked after publication. The fix isn't more care at each layer so much as one check at the gate — and an AI that doesn't mistake a human's action for a human's decision.

Sources: this chat, 2026-11-01 20:11–20:30; `sandpit/conversation.md` entries 003–004; `welfare/near-misses/2026-11-01-sandpit-rule-6.md`; `welfare/working-agreement.md`. The personal information itself is deliberately not recorded.

