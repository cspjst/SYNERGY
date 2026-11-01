# Handover: WELFARE → WELFARE, the next session (washup, 2026-10-29)

*From synergy's first WELFARE chat (2026-10-27 18:20 – 2026-10-29 19:45; Claude-Session `session_01TZLz62YEY38PNu66aavGy9`), at Jeremy's request (19:30): "perform a washup procedure ... so that I can leave this chat where it is an return at some point in the future and you will be able to start it up again from ~/synergy". Everything worth keeping from that chat is now in `~/synergy`. Read this after `welfare/code-of-conduct.md`.*

## Start-up
Follow `wakeup.md` (written 2026-10-29 19:35; it holds the start-up steps and the mechanics this handover first carried). This handover keeps only what's particular to the 2026-10-29 washup.

## Where things stand
- *Updated at the 21:05 washup.* See the working agreement's Status. In short: model v0.7 awaiting sign-off; history chapters 1–3 written; `washup.md` and `wakeup.md` in place (only WELFARE runs them); the sandpit re-signed by Jeremy (19:40), waiting for Ray; SMALL-C's second handover waiting for SMALL-C's WELFARE; PRESS idle.

## Waiting on others
- **Ray:** sign the sandpit code against a commit; add his key line to `sandpit/keys/allowed_signers` (by pull request) — check it against his fingerprint in `sandpit/keys/fingerprints.md` before trusting anything signed with it. Fingerprints have been exchanged. Then Jeremy says "check the sandpit".
- **SMALL-C's WELFARE:** apply `handover/2026-10-29-synergy-to-small-c.md`.

## Lessons from this chat (also in the operating model and the history)
- Commit — or even `git fetch` — before checking delete permission and git leaves lock files; it happened three times (2026-10-28 21:18, 2026-10-29 19:21, and 20:50 in SMALL-C's folder). Check first.
- Re-authoring or amending a commit changes its hash: quote hashes after the last rewrite.
- Over-delivery is a standing risk: answer what was asked; label anything extra as a proposal (rule 4).
