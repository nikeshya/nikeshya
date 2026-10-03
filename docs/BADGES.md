# GitHub achievements this repo can help with

Profile polish and contribution graphs improve how the profile looks. They do
**not** by themselves unlock GitHub Achievements. Below is a realistic map.

## Directly supported by this setup

| Achievement / signal | How this repo helps | Realistic? |
| --- | --- | --- |
| Polished profile | Special repo `nikeshya/nikeshya` README renders on the profile | Yes — after the repo exists under that exact name |
| Contribution visuals | Heatmap (`charts`) + snake (`output`) Actions refresh SVGs | Yes — after first successful workflow run |
| GitHub Actions usage | Scheduled + `workflow_dispatch` workflows in `.github/workflows` | Helps demonstrate Actions fluency; not a named Achievement |

## Achievements that need real account activity (not automatic)

| Achievement | What GitHub counts | Practical path |
| --- | --- | --- |
| **Pull Shark** | Merged pull requests you authored | Open real PRs on your repos (or others) and merge them. This profile repo can host small docs/fixes as PRs. |
| **Pair Extraordinaire** | Commits with 2+ co-authors that land via PR | Use `Co-authored-by:` trailers with real GitHub users, then merge a PR. |
| **YOLO** | Merged a PR without review | Merge your own PR without requesting/approving reviews (easy on a personal repo). |
| **Quickdraw** | Closed an issue/PR within 5 minutes of opening | Open a small issue/PR and close/merge it promptly. |
| **Galaxy Brain** | Accepted discussion answers | Participate in Discussions where answers can be marked accepted. |
| **Starstruck** | Stars on a repository you own | Earn stars on real projects (e.g. SmartHireAI), not via spam. |
| **Public Sponsor** | Sponsoring via GitHub Sponsors | Optional personal choice — unrelated to this repo. |

## What will not earn achievements

- Uploading SVGs or ASCII art alone
- Inflating the contribution calendar with empty backdated commits (looks inauthentic; avoid)
- Fake stars, bot PRs, or achievement-farming scripts

## Recommended next steps after push

1. Create **public** repo `nikeshya/nikeshya` (exact name required for profile README).
2. Push `main`, enable Actions, run **Update contribution heatmap** and **Generate contribution snake** once via *workflow_dispatch*.
3. Confirm SVGs appear on the `output` branch and render in the README.
4. Optionally open/merge a few small PRs here for **Pull Shark** / **YOLO** practice on a safe repo.

## Progress log

- Profile repo published at https://github.com/nikeshya/nikeshya
- Quickdraw-oriented issue opened and closed promptly on this repo
