# personal-website-pages — DO NOT TOUCH

> **Never edit this repository by hand.**

Public GitHub Pages host for **https://zackli.ai**. Source stays private in [`personal-website`](https://github.com/zhiyuan8/personal-website).

## How it works

- Edit the site in [`personal-website`](https://github.com/zhiyuan8/personal-website) (private).
- Redeploy from this repo: Actions → **Build from private source** → Run workflow.
- That job clones the private source, builds `out/`, and force-pushes `gh-pages`.
- GitHub Pages serves `gh-pages` at `zackli.ai`.

## Rules

- Do not commit or open PRs here — the next deploy overwrites `gh-pages`.
- Change the site in the private source repo, then push `main`.
- The only manual setting here is Pages (custom domain `zackli.ai` / Enforce HTTPS).
