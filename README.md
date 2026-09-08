# Jason’s personal site

A simple static website (HTML + CSS, tiny bit of JavaScript) for GitHub user [jason-p919](https://github.com/jason-p919). It is meant to be easy for a total beginner to edit, and safe to keep public.

Live URL (after you turn on GitHub Pages): **https://jason-p919.github.io/site/**

## What’s on the site

| Page | File | What it is |
|------|------|------------|
| Home | `index.html` | Intro and links to every section |
| Work | `work.html` | AI projects + NI / LabVIEW / GPU / local models cards |
| Personal | `personal.html` | Impala Callaway, Fuji gallery placeholders, Midjourney placeholders |
| Reading | `reading.html` | Books with short notes (example entries marked) |
| Movies | `movies.html` | Letterboxd-style watched list (placeholders) |
| Contact | `contact.html` | Business email + privacy note |
| Build log | `build-log.html` | Dated changelog |

Shared look-and-feel lives in `css/styles.css`. The mobile “Menu” button is wired in `js/main.js`.

## How to edit a page

1. Open the HTML file you want (for example `work.html`) on GitHub or on your computer.
2. Change the text inside the tags. You do **not** need React, npm, or a build step.
3. Keep links relative (`work.html`, `css/styles.css`) so the site works under `/site/` on GitHub Pages.
4. Commit and push. If Pages is enabled from this branch, the site updates in a minute or two.

**Contact email:** In `contact.html`, replace `YOUR_EMAIL@example.com` in both the `mailto:` link and the visible text. Do not invent or commit anyone else’s address.

**Photos:** Add compressed images under something like `images/`, then point `<img src="images/...">` at them. Avoid huge binaries in git.

## How GitHub Pages works

1. Open the repo **Settings → Pages**.
2. Under “Build and deployment”, set Source to **Deploy from a branch**.
3. Choose the branch you want (often `main`) and folder **/ (root)**.
4. Save. GitHub will publish at `https://jason-p919.github.io/site/`.

The empty `.nojekyll` file tells GitHub not to process the site with Jekyll, so files and folders that start with underscores (if you add any later) still work.

## SECURITY

- This repository is **public**. Anything you commit can be seen by the world.
- **Never** commit tokens, API keys, passwords, private keys, `.env` files, or confidential work data.
- Do not put secrets in HTML comments, JS, or “hidden” files — public still means public.
- The contact page uses a placeholder email on purpose until you deliberately add a real one.

## License

Apache License 2.0 — see [LICENSE](LICENSE).
