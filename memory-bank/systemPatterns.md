# System Patterns: Meadowist

## Architecture Status
Meadowist is a **static website** — a single home page (`index.html`) styled with `style.css`. No server-side code, build step, or framework is required.

## Site Structure
```
meadowist/                  # repo root
├── index.html              # home page
├── style.css               # styling (neutral background, green accents)
├── meadowist.png           # site logo (1408x768)
├── meadowist-small.png     # small site logo (1380x752)
├── gsp-events.png          # Work Party Notifier project logo (813x737)
└── memory-bank/            # project knowledge base
```

## Design Patterns
- **Static site** — plain HTML + CSS, zero dependencies, deployable to any static host
- **Project card grid** — new projects are added as new `.project-card` elements in `section.projects`
- **External links** — project cards use `target="_blank" rel="noopener"` to open subdomains in new tabs
- **Design language** — subtle neutral background (`#fafafa`), white card with soft shadow, forest-green accents (`#1b5e20`, `#2e7d32`, `#4e7c4e`)

## Key Technical Decisions
- **Plain static HTML/CSS** (no framework) — chosen for simplicity; the site only needs to display a logo, mission statement, and project links

## Coding Conventions
- No JS yet; if added, would follow vanilla, dependency-free approach
- Responsive mobile layout via CSS media queries (`@media (max-width: 600px)`)

## Design Principles
- Nature-inspired: green accents evoking parks and forests
- Clean, uncluttered layout with a clear mission statement up top
- Simple project cards that are easy to scan and click