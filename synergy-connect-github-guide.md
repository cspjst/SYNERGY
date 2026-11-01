# How to connect Claude to GitHub

*Owned by synergy's WELFARE. Written 2026-10-27 for someone doing it for the first time. Tested once: Jeremy linked GitHub between 20:33 and 20:46 that evening, and Claude pushed to `cspjst/CLAUDE` (since renamed `cspjst/SYNERGY`) straight after. The screens may change; where this guide guesses, it says so.*

## Why you'd want it
With GitHub linked, Claude can push your project's commits to GitHub for you — the backup — instead of you doing it by hand. Without it, Claude can still read and write the files on your computer, but it can't send them to GitHub.

## What you need
- A GitHub account, with the repository already created on GitHub (for synergy: `cspjst/SYNERGY`).
- The Claude app, or claude.ai in a browser, signed in.

## The steps

1. **Open Claude's settings.** Click your name or initials in the bottom-left corner, then **Settings**.
2. **Go to Connectors.** Choose **Connectors** in the settings list.
3. **Find GitHub and connect it.** Click **Connect** (or **Link** — *the exact word is a guess*) beside GitHub.
4. **Sign in to GitHub.** A GitHub page opens in your browser. Sign in if it asks.
5. **Authorise Claude.** GitHub asks whether Claude may access your account. Say yes.
6. **Choose the repositories.** GitHub offers to install the **Claude GitHub App**. If the repository is in your own account, you can grant this yourself:
   - choose **Only select repositories** — the safer choice;
   - pick your project's repository;
   - click **Install**.
7. **Go back to Claude** and tell the chat it's done. Claude tries again and reports what happened.

## If it doesn't work
- **Claude says the repository isn't reachable:** it's probably not in the list you chose in step 6. On GitHub, go to Settings → Applications, open the Claude app, and add the repository.
- **The repository belongs to an organisation:** an organisation administrator may have to approve the request before Claude can reach it.
- **Anything else:** ask Claude to quote the exact error, not to guess.

## How Claude uses it (synergy's setup)
- The project's files live on your computer (for synergy, `~/synergy` — the oracle).
- Claude commits there as `Claude-SYNERGY-WELFARE`.
- The shell Claude uses on your computer has no GitHub password, so Claude carries the commits across to its own workspace and pushes from there, using the link you made above.
- Afterwards Claude brings your computer's copy level with GitHub, so all three agree.

## The quick alternative
If you'd rather not link GitHub, push from your own Terminal with `git push`. Claude's commits will be waiting.

Sources: Claude Help Center, "Use the GitHub integration" (support.claude.com/en/articles/10167454); synergy's WELFARE chat, 2026-10-27 20:32–20:47.
