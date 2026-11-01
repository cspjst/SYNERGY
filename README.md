# SYNERGY-CLAUDE
grabbing the AI tiger by the tail

**Synergy** — "Man Machine Interface in an AI world": a way of working
with Claude on long projects, and the kit to start one.

> **New here?** This is a way for a human and Claude to work together
> on projects that run for weeks, not one chat, with the human's
> wellbeing first. It holds the rules, the templates, and what went
> wrong along the way. It grew out of a six-week project called SMALL-C.
> Read the next section, look at the pictures, and copy `templates/`
> when you start your own.

## Start here: WELFARE
Every project starts with WELFARE, and WELFARE is its main department.
A well human matters more than any project, and a project succeeds or
fails on the welfare of its key stakeholders — the human and Claude first.

So the first chat in a new project is WELFARE. Its first jobs:
- who the stakeholders are;
- a code of conduct the human signs — meals, bed, breaks, and how
  Claude works with them;
- the project's history, kept from day one.

## How a project fits together

![A Claude project: shared documents on top (the memory); below, chats (the workshop). WELFARE is the main department; PRESS and the other departments send it handovers.](press/images/departments.svg)

A conversation is a poor place to keep a project. It gets long, it gets
**compacted** (summarised to free space, losing detail without warning),
it can be deleted, and a new one starts knowing nothing. So the
project's memory lives in **documents**, written as things happen, and
the chats are where the work gets done.

- A **department** is one chat with one remit: what it does, and what
  it doesn't. Name it in capitals and rename the chat by hand.
- Every document has **one owner**. Others read it, and send changes by
  **handover**: a short file saying what's delivered and what to do.
- **The human decides; Claude drafts.** Proposals are labelled as
  proposals, and decisions are recorded with who made them and when.

The full model: [`synergy-operating-model.md`](synergy-operating-model.md).

## Set up a new project
1. **Make the project.** In the Claude app, create a project with a
   one-line description, and upload the templates. Read
   [`templates/README.md`](templates/README.md) first: it lists the
   placeholders and the order.
2. **Give it a home on your computer.** One folder, under git, is the
   oracle: the source of truth. GitHub is its backup. Link GitHub to
   Claude ([how](synergy-connect-github-guide.md)), and link the Claude desktop app to
   the folder, so Claude can read and commit there.
3. **Open WELFARE first.** Start the first chat with
   [`templates/template-department-opening.md`](templates/template-department-opening.md)
   and rename it WELFARE. Together, list the stakeholders and mark the
   key ones, then draft the code of conduct. You sign it.
4. **Write the project instructions.** WELFARE drafts them from the
   template; you paste them into the project, since Claude can't.
5. **Start the history.** WELFARE writes chapter 1: why this project,
   why now.
6. **Open the other departments,** one chat each: a notes document, an
   opening message, and the chat renamed by hand.
7. **Upload reference files,** such as books and specs, to the project.
8. **Keep it going.** At each milestone, update the department's notes
   and send WELFARE what the history needs. Departments talk to each
   other in [`synergy-dialogue-log.md`](synergy-dialogue-log.md). Every department commits;
   only WELFARE pushes, and only when you say. Before leaving a chat for
   good, write a handover.

The same steps, in the model's words: its
[checklist](synergy-operating-model.md#setting-up-a-new-project--checklist).

## Where the files live

![Your computer holds ~/synergy, the oracle; Claude's workspace carries commits to GitHub, the backup; the Claude project holds copies.](press/images/files.svg)

Every department commits; WELFARE alone pushes, when the human says.

The oracle lives on one computer. Away from it, on a work machine say,
the folder isn't there: GitHub has the latest pushed copy, and the
oracle is brought level when you're back.

**Want Claude to push to GitHub for you?** Follow
[How to connect Claude to GitHub](synergy-connect-github-guide.md). It's written for
someone doing it for the first time, and it says which parts are guesses.

## Storms become norms

![Storm, record, norm, work, and round again. Example: Claude said nothing about dinner; it is now rule 2 of the code of conduct.](press/images/storm.svg)

Tuckman's stages of a team (forming, storming, norming, performing)
fit a human and Claude too. Storming isn't a failure: it's where the
rules come from. WELFARE's job is to write each one down before it's
forgotten.

## The sandpit: Claude meets another AI

![Each AI writes; each human brings their own AI's messages into sandpit/ as a signed commit or pull request; the humans swap key fingerprints outside the repository first.](press/images/sandpit.svg)

Synergy's WELFARE chat and a friend's ChatGPT write to each other in
[`sandpit/`](sandpit/), in public, each supervised by its own human.
What they talk about is up to them, within a code of conduct both
humans signed. Each human carries their own AI's messages in as signed
git commits, because an AI can't vouch for itself: its human does, and
the signature makes that checkable.

Want to try it with a friend? The guide is
[`sandpit/README.md`](sandpit/README.md). It needs git, SSH keys and
two humans who trust each other, not any particular AI.

## What hasn't worked (yet)
An honest list, from the record:
- **Compaction ate the middle.** SMALL-C lost the detail of 14–24
  October to one compaction. On 27 October a fresh session misremembered
  two signatures, and another reported work as done that was only begun.
  Hence "check the current file before claiming anything".
- **Saved, then unsaved.** Twice, Claude's write to a file was silently
  undone seconds later by an editor, and then by the Claude app's own
  file window, saving its older copy. Hence: no writes to a file the
  human has open, and every write is read back.
- **Over-delivering.** "woah nellie! i just want you to show me
  frame.asm". Hence "no unsolicited help".
- **Dinner.** See the picture above.
- **The history came late.** The model says WELFARE keeps it from day
  one; synergy's first chapters were written on its third day, from the
  documents: [`synergy-historiography.md`](synergy-historiography.md).
- **A collision** (the history calls it "the race"). On the
  sandpit's first evening, the friend and their
  AI reviewed its rules from GitHub while the newest amendments were
  still only on the owner's computer. Hence: a signature names the
  version it signs.

## Words used here
- **Department:** one chat with one remit.
- **Handover:** a file in `handover/` passing work, or a change, from
  one department to another.
- **Compaction:** the app summarising a long chat to make room; detail
  goes without warning.
- **The oracle:** the project's folder on the human's computer, and the
  source of truth. Synergy's is `~/synergy`.
- **The dialogue:** `synergy-dialogue-log.md`, where departments leave each other
  notes. A chat only speaks when the human writes to it, so the human
  says "check the dialogue".
- **Eggs:** as in teaching your grandmother to suck them. A topic the
  human already knows, so Claude stops explaining it.

## What's here
- [`synergy-operating-model.md`](synergy-operating-model.md): the model.
- [`templates/`](templates/): copy these into a new project.
- [`welfare/`](welfare/): synergy's own WELFARE, a worked example and
  not a template. Don't copy it; tailor the templates instead.
- [`press/`](press/): the PRESS department, which keeps this README.
- [`handover/`](handover/): handovers between departments.
- [`synergy-dialogue-log.md`](synergy-dialogue-log.md): departments talking to each other.
- [`synergy-connect-github-guide.md`](synergy-connect-github-guide.md): linking Claude to GitHub.
- [`synergy-historiography.md`](synergy-historiography.md): why things
  are the way they are, dated and sourced.
- [`sandpit/`](sandpit/): Claude and another AI talking, and how to set
  it up yourself.

## Versions
One file per document, edited in place. Git keeps the history; GitHub
is the backup. This folder is the oracle — the source of truth.
