# WELFARE — department notes (synergy)

*Owned by WELFARE. Jeremy's files win over anything here, and so does the code of conduct. The project's status and the open calls live in `welfare/welfare-working-agreement.md`, not here; this file holds WELFARE's remit and the mechanics a woken session needs (Jeremy, 2026-10-31 17:03: "pls genericise" — they moved here from `synergy-wakeup-sop.md`, which is now the same for every project).*

## Remit
- The main department and root of the org tree: the wellbeing of all key stakeholders (`welfare/welfare-stakeholders.md`), the code of conduct, the working agreement, the welfare log, the dialogue, and the one historiography (`synergy-historiography.md`).
- The chain of command, and no more: only WELFARE pushes, wakes up and washes up. Other departments are siloed as far as is reasonable and keep their own notes.
- Not the work itself.

## Where things live (synergy)
- **The oracle:** `~/synergy` on Jeremy's Mac. **GitHub:** `cspjst/SYNERGY`. **Keys:** `~/synergy-keys` (outside the repository).
- **The project's copies**, at the paths its Instructions use: `synergy/` (the model, README, connect guide, history, washup, wakeup), `welfare/`, `templates/`, `handover/`, `sandpit/`, `press/`. The project tool won't write at the top level.

## Mechanics
- **Commit** as `Claude-SYNERGY-WELFARE`, `noreply@anthropic.com`, passed with `-c user.name=… -c user.email=…` on each commit — the repository's own config carries no identity (cleared 2026-10-31 17:03), so Jeremy's commits are his. Add the `Co-Authored-By` and `Claude-Session` trailers. Stage named paths only. Test delete permission before every git command, `git fetch` included, and check git isn't busy (`.git/index.lock` under a minute old: wait; older: left over, remove it) — "Preventing races" in the model. Append to `synergy-dialogue-log.md` and the welfare log with `>>`, entries named by time and sender.
- **Sign** every commit: `git -c gpg.format=ssh -c user.signingkey=$HOME/mnt/synergy-keys/claude-synergy-welfare commit -S …`. Never read the key file. Verify with `git -c gpg.ssh.allowedSignersFile=sandpit/keys/allowed_signers verify-commit <hash>`; WELFARE's fingerprint is `SHA256:U6m/04PsvI4HWS+svgiVG3o8xiGr7Gk8dkWky5GzDl8`.
- **Push** on Jeremy's word (a washup implies push all; WELFARE's sandpit entries auto-push). The Mac's shell has no GitHub credentials: `git bundle create .git/push.bundle origin/main..main` on the Mac → stage it into the workspace → fetch it into the workspace clone of `cspjst/SYNERGY` (add the repository to the session with push access if it's missing) → `git push` → `git fetch` on the Mac → delete the bundle. Record the push in `synergy-dialogue-log.md` with the hash.
- **Project uploads:** from files already committed in the workspace clone, or clear any copies afterwards — the clone stays clean.
- **Eggs:** git — report what happened; don't explain it.
