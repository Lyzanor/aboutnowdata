# About Now Data

Static single-file site for the About Now Data framework.

## Structure

- `index.html`: the whole site. HTML, CSS, JS, and the client-side `.zip` download all live here.
- `learn.html`: explanation page for the About Now Data system.
- `LICENSE`: repository license.

## Update Guide

Most future edits should happen in one place inside [index.html](/Users/lyzanor/Documents/Me/Data/Projects/Invento%20de%20la%20IA/Data/Web%20About%20Data%20Now/Data/Github%20-%20About%20Data%20Now/index.html):

- Search for `const HERO_CARDS = [` in the script near the bottom.
- Each card object controls:
  - tab label
  - file or folder label
  - editable content
  - contextual description shown below the stack
  - copy behavior

If you need to change the homepage copy outside the interactive stack:

- edit the hero text directly in the HTML section near the top
- edit the lower sections (`What it is`, `Feedback`, footer) directly in the markup

## Design Notes

- The hero stack is rendered from `HERO_CARDS` so content is not duplicated across HTML and JS.
- The active card grows, becomes editable, and drives the detail panel below it.
- Copy buttons always read the live edited content, not a stale template.

## Local Preview

Run a static server from the repo root:

```bash
python3 -m http.server 4173
```

Then open:

```bash
http://127.0.0.1:4173/index.html
```

## Deploy

GitHub:

```bash
git push origin main
```

Vercel production:

```bash
vercel deploy --prod -y
```
