# Working in this repo

`n8n-nodes-halopsa`, an n8n community node for HaloPSA tickets, notes and attachments. `README.md`
explains what it does and how to install it from a local tarball.

- The package is not published to npm. Don't publish it or change its version without Mike's
  explicit approval.
- There are no tests and no lint script; the check is a clean TypeScript build: `npm install`, then
  `npm run build`. There is no lockfile, so `npm ci` fails, and `npm install` creates an untracked
  `package-lock.json` that should not be committed by accident.
- This repo is public. Never commit a Halo tenant URL or subdomain, an OAuth client ID or secret, or
  real ticket data. Client work lives in private repos; don't copy any of it here.
- Start from the default branch, `main`. When the work is done, open a pull request into `main` and
  tell Mike it is ready to merge. Finished work should never be left on a branch without a pull request.
