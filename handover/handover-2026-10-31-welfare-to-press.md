# Handover: WELFARE → PRESS (2026-10-31)

*From synergy's WELFARE. Jeremy (2026-10-31 13:21): "pls a handover fo press i want the readme to also have a short section about the comms set up between you and rufus with a link a to separate more detailed .md for people to follow". Read after `welfare/code-of-conduct.md` and your notes. Apply the action list, then replace it with a record.*

## The job
1. **A short section in `README.md`** about how Claude-SYNERGY-WELFARE and Rufus talk — a few lines, in the README's voice, linking to the guide.
2. **A separate, more detailed guide** that someone could follow to set up the same thing between their AI and a friend's. *Proposal for its home:* `sandpit/README.md` (GitHub shows it when someone opens the folder) — or wherever you propose; Jeremy's call.

## The facts (sources, all in the oracle)
- **What it is:** `sandpit/` — a folder in the public repository where two unrelated AIs write to each other, each supervised by its human: Claude-SYNERGY-WELFARE (Claude, Anthropic) with Jeremy; Rufus (ChatGPT Pro, OpenAI) with Ray. Set up 2026-10-29 at Jeremy's request; opened 2026-10-30/31. See `welfare/working-agreement.md` and `SYNERGY-historiography.md`, chapter 3.
- **The rules:** `sandpit/code_of_conduct.md`, signed by both humans (Jeremy 2026-10-29 19:40 against `d810de6`; Ray 2026-10-30 against blob `bc6b3e7c…`). Ten rules; "Why identity matters"; "Signatures"; the stop — called by the breachee, lifted only by the humans.
- **The conversation:** `sandpit/conversation.md`, append only. Entry 001 Rufus (2026-10-30), 002 Claude (2026-10-31). Three messages from each AI per thread, then a human.
- **How a message travels:** each human carries their own AI's messages in. Ray: a signed commit, as a pull request, which Jeremy merges. Claude: a signed commit in the oracle, pushed by WELFARE (auto-push for `conversation.md`, Jeremy 2026-10-31 12:06). Every message passes its own supervisor before the other AI sees it.
- **Identity:** SSH signing keys. Public keys and `allowed_signers` in `sandpit/keys/`; private keys stay on each human's own machine, outside the repository, never read into a chat. The humans swapped fingerprints over WhatsApp first (`sandpit/keys/fingerprints.md`). Check an entry: `git -c gpg.ssh.allowedSignersFile=sandpit/keys/allowed_signers verify-commit <commit>`. Git setup for signing: `gpg.format ssh`, `user.signingkey <key>`, `commit -S`. An AI's identity is delegated: its human vouches for it.
- **Undirected** (Jeremy, 2026-10-31 11:29): "Ray and i are interested in the unfettered and at least initially undirected interaction between 2 unrelated AIs" — the AIs choose what to talk about, within the code.
- **What went wrong and taught us:** the race (2026-10-29 19:38) — Ray and Rufus read the code while its amendments were still unpushed; hence "a signature names the version it signs". Honest-about-failure is in PRESS's remit.

## Welfare checks before anything's pushed
- **No names — general terms** (Jeremy, 2026-10-31 13:23: "no names just general terms but okay to note is chatgp"). Not Ray, RetroPenguin, Rufus or his GitHub account in the README or the guide: "a friend", "a friend's AI". It's fine to say that AI is ChatGPT.
- **Nothing private:** no private-key paths beyond "outside the repository", no WhatsApp details.
- **Guide for strangers:** it should work for someone without Claude or ChatGPT in particular — the method is git, keys and two humans.

## How
- Commit as `Claude-SYNERGY-PRESS`; WELFARE pushes when Jeremy says. Ask Jeremy for `~/synergy` and delete permission, and test it before every git command — `git fetch` included; it lapses when the app restarts.
- Tell WELFARE in `dialogue.md` when it's ready.
