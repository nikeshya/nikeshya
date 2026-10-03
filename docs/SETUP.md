# Setup: publish as `nikeshya/nikeshya`

This checkout is ready to become the special profile repository. GitHub only
renders a profile README from a **public** repo named exactly
`nikeshya/nikeshya` owned by user `nikeshya`.

## Option A — GitHub CLI (recommended)

```bash
gh auth login
gh repo create nikeshya/nikeshya --public --source=. --remote=github --push
```

If `origin` already points elsewhere:

```bash
git remote add github https://github.com/nikeshya/nikeshya.git
git push -u github main
```

## Option B — GitHub UI

1. Sign in as **nikeshya**.
2. Create a new **public** repository named **nikeshya** (no README/license/gitignore).
3. Push this branch:

```bash
git remote add github https://github.com/nikeshya/nikeshya.git
git push -u github main
```

## After the first push

1. Open the repo **Actions** tab and allow workflows if prompted.
2. Run **Update contribution heatmap** → *Run workflow*.
3. Run **Generate contribution snake** → *Run workflow*.
4. Confirm generated branches:
   - `charts`: `contributions.svg`, `contributions-dark.svg`
   - `output`: `github-contribution-grid-snake.svg`, `github-contribution-grid-snake-dark.svg`
5. Visit `https://github.com/nikeshya` — the README should appear at the top.

## Private contributions on the heatmap

`GITHUB_TOKEN` from Actions only sees what the default token can see. To include
private contributions in gcchart, add a PAT with `read:user` (+ `repo` if needed)
as a repository secret and point the heatmap workflow `github_token` input at it.
