# ezra-public

Public static site for Ezra-generated artifacts, intended for GitHub Pages.

## What this repo contains

- A minimal landing page at `index.html`
- A custom `404.html` so broken links fail gracefully
- A GitHub Actions workflow that deploys the site to GitHub Pages

## Publishing model

- Repository owner: `ezramigdali`
- Repository visibility: `public`
- Expected remote: `git@github-ezra:ezramigdali/ezra-public.git`
- Deployment target: GitHub Pages via GitHub Actions

## Local push flow from WSL

After the empty GitHub repository exists, run:

```bash
/home/openclaw/.openclaw/workspace/bin/ezra-public-push
```

That script initializes the repo if needed, sets the `origin`, commits the scaffold, renames the branch to `main`, and pushes to GitHub.
