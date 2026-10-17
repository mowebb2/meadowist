# Progress: Meadowist

## Project Status
**Phase:** Home page built — ready for commit and deployment
**Status:** Static site complete; no commits pushed to GitHub yet

## What Works
- **Home page** (`index.html` + `style.css`) at the repo root:
  - meadowist logo displayed prominently
  - Mission statement: *"Resources for maintaining Seattle's urban forests and parklands"*
  - "Projects" section with a link card for **Work Party Notifier** at `gsp-events.meadowist.dev`
  - Subtle neutral background with forest-green accents (less green per user feedback)
  - Responsive layout (mobile-friendly)
- Repository contains all logo assets:
  - `meadowist.png` (site logo)
  - `meadowist-small.png` (small site logo)
  - `gsp-events.png` (Work Party Notifier logo)

## What's Left to Build
- [ ] Initial commit to GitHub
- [ ] Deploy `meadowist.dev` (Cloudflare Pages, GitHub Pages, or similar static host)
- [ ] Add more project cards as new meadowist projects launch

## Known Issues / Blockers
- gsp-events.meadowist.dev needs to be live for the project link to work (source at `/Users/mwebb/Projects/gsp/gsp-event-monitor`)
- Repository has no commits yet — first commit is pending

## Current Roadmap
1. ✅ Define vision — mission statement confirmed: environmental restoration, local parks, planting, stewardship
2. ✅ Build home page — logo, mission, project card for gsp-events
3. ⏳ Commit and deploy — push to GitHub and set up hosting for `meadowist.dev`
4. ⏳ Add more projects — expand the card grid as new projects launch

## Decisions Made
- **Mission statement:** "Resources for maintaining Seattle's urban forests and parklands"
- **Tech approach:** Plain static HTML + CSS, no framework, no build step
- **Design language:** Subtle neutral background (`#fafafa`) with forest-green accents
- **Project section:** Card grid with logo, name, description, and external link per project

## Milestones
| Milestone | Status |
|-----------|--------|
| Repository created | ✅ Done |
| Memory bank initialized | ✅ Done |
| Home page built | ✅ Done |
| Initial commit | ⏳ Pending |
| Deployed to meadowist.dev | ⏳ Pending |