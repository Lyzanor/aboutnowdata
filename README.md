# About Now Data

*An agentic system, built for real people.*

Memory systems with context you can inspect line by line.

## Links

- [Live site](https://aboutnowdata.vercel.app)
- [Explanation](https://aboutnowdata.vercel.app/learn.html)
- [Examples](https://aboutnowdata.vercel.app/examples.html)
- [MIT License](./LICENSE)

## What It Is

About Now Data is a simple memory system based on Markdown.

It keeps identity, current priorities, and durable knowledge separate enough to remain legible for both humans and agents.

The goal is not just better memory inference. The goal is memory that stays inspectable, editable, portable, and focused.

## Three Layers

### `About.md`

Stable, defining, foundational.

This is where identity, values, rules, and boundaries live.

### `Now.md`

Brief, current, actionable.

This is where active priorities, recent activity, next steps, risks, and opportunities live.

### `Data/`

Structured depth.

This is where projects, references, notes, tools, and supporting detail live without polluting the core.

## Starter Shape

```text
About.md
Now.md
Data/
```

Minimal by design.

One About file. One Now file. One Data folder.

## This Repository

This repo contains the public site for About Now Data.

```text
index.html      Home
learn.html      Explanation
examples.html   Examples
shared.css      Shared styling
LICENSE         MIT license
```

The site is intentionally lightweight and static.

## Local Preview

Run a static server from the repo root:

```bash
python3 -m http.server 4173
```

Then open:

```text
http://127.0.0.1:4173/index.html
```

## Deploy

Production deploy:

```bash
vercel deploy --prod -y
```

## Why It Exists

Most memory systems optimize for hidden capture, silent consolidation, and black-box recall.

About Now Data takes the opposite position.

Memory should be legible.

Stable context and changing context should not be mixed.

Human control matters more than hidden cleverness.

## License

MIT
