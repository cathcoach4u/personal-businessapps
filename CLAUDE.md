# Personal Business Apps — Apps Hub

## Working Style
- Don't apologise — just action
- Push to main — don't create PRs unless asked
- Australian English, no uppercase headings

## What is this
The central launch page for Baker and Cath family personal apps. Single page with PWA capability. Separate Family Dashboard page available for organized access to family, Japan trip, and coaching portal apps.

## Architecture
- **URL**: cathcoach4u.github.io/personal-businessapps/
- **Stack**: Single HTML page, no database, no frameworks
- **PWA**: Manifest + service worker for home screen install
- **Design**: Gradient header (teal to purple), 3-column tile grid
- **Cost**: Free (GitHub Pages hosting only)

## Sections & Apps

### index.html — Personal Hubs
| App | URL | Icon |
|-----|-----|------|
| Baker Hub | cathcoach4u.github.io/personal-baker-hub/ | Teal B |
| Baker AI | cathcoach4u.github.io/personal-baker-hub/ai.html | Purple B |
| AisleMate | cathcoach4u.github.io/personal-baker-hub/shopping.html | Blue Sh |
| Cath Hub | cathcoach4u.github.io/personal-cath-hub/ | Teal C |
| Cath AI | cathcoach4u.github.io/personal-cath-hub/ai.html | Purple C |
| Morning | cathcoach4u.github.io/personal-cath-hub/morning.html | Yellow sun |
| Trip Planner | cathcoach4u.github.io/personal-baker-hub/japan-2026.html | Orange JP |
| Japan AI | cathcoach4u.github.io/personal-baker-hub/japan-ai.html | Purple J |

### family-dashboard.html
Separate page with family-focused layout:

**Baker Family Priorities** — Shopping, Trip Planner, Japan AI

**Family Based Apps** — Baker Hub, Baker AI

**Cath Apps** — Cath Hub, Cath AI, Morning

**Coaching Portal** — cathcoach4u.github.io/coach4Uapp-dashboard/ (C4U icon)

## Related Repositories
| Repo | Purpose | CLAUDE.md |
|------|---------|-----------|
| personal-baker-hub | Baker family dashboard | Yes |
| personal-cath-hub | Cath's personal dashboard | Yes |
| internal-coach4u-hub | Coach4U internal hub + bot | Check |
| client_IAS | IAS client app | Check |

## Key Files
| File | Purpose |
|------|---------|
| index.html | Main apps hub page (entry point) |
| family-dashboard.html | Family-organized dashboard (separate page) |
| manifest.json | PWA manifest |
| sw.js | Service worker for offline/caching (v2) |
| icon-192.svg / icon-512.svg | PWA icons |
| CLAUDE.md | This file — project memory |

## Adding a New App
1. Add a tile in the appropriate section in index.html
2. Use the same tile HTML pattern (app-tile class)
3. Choose an icon colour and letter/symbol
4. Tag as PWA, WEB, or LINK
5. Push to main

## If Moving Away From Claude
- This is a static HTML page with no AI dependencies
- Any developer or AI tool can edit it
- Rename CLAUDE.md to PROJECT.md
- Everything keeps working as-is
