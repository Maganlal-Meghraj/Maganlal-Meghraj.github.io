# Maganlal-Meghraj.github.io

Personal profile site of **Pushkal Guha Choudhury**, a backend engineer working on lending, billing and logistics systems.

**Live:** https://maganlal-meghraj.github.io/

## What's on it

- **Hero:** availability, a one-line intro and a small terminal card.
- **Highlights:** four headline numbers from recent work.
- **Career, as a commit log:** roles and education drawn as a `git log --graph`, newest first.
- **Selected work:** case studies written as context, approach and result.
- **Skills and contact.**

The page follows the system light/dark setting, and a toggle in the nav overrides it (the choice is saved in `localStorage`).

## Stack

Plain HTML and CSS with a few lines of vanilla JavaScript. There is no build step or dependencies; fonts (Geist, Geist Mono) load from Google Fonts.

```
index.html   page content and the small scripts (theme toggle, "more changes" toggle)
style.css    all styles; colours are light-dark() tokens on :root
```

## Run locally

Serve the folder with any static server, for example:

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000.

## Deploy

GitHub Pages serves the `main` branch from the repo root. Pushing to `main` redeploys within about a minute.

When `style.css` changes, bump the version query on its link in `index.html` (`style.css?v=N`) so browsers don't keep a cached copy.
