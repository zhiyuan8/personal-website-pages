# personal-website-test — DO NOT TOUCH

> **⚠️ Never edit this repository by hand.**

This repo is a **deploy target only** for the staging site
**https://test.zackli.ai**. It exists solely because GitHub Pages allows only
one site / custom domain per repository, so staging cannot share
[`personal-website`](https://github.com/zhiyuan8/personal-website) (which
serves production at https://zackli.ai).

## How it works

- All source code lives in
  [`personal-website`](https://github.com/zhiyuan8/personal-website).
- Every push to its `main-test` branch runs
  [`deploy-staging.yml`](https://github.com/zhiyuan8/personal-website/blob/main-test/.github/workflows/deploy-staging.yml),
  which builds the site and **force-pushes the output to the `gh-pages` branch
  here**, wiping whatever was there before.
- GitHub Pages serves that `gh-pages` branch at `test.zackli.ai`.

## Rules

- Do **not** commit, edit files, or open PRs here — changes will be
  overwritten on the next staging deploy.
- To change the staging site, push to `main-test` in
  [`personal-website`](https://github.com/zhiyuan8/personal-website).
- The only manual thing ever done here is the Pages settings
  (custom domain / Enforce HTTPS).
