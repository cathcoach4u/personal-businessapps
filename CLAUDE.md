# Personal Business Apps — Apps Hub

## Working Style
- Don't apologise — just action
- Push to main — don't create PRs unless asked
- Australian English, no uppercase headings

## What is this
The central launch page for all Baker family and Coach4U apps. A single page with tile links to every app, installable as a PWA on the home screen.

## Architecture
- **URL**: cathcoach4u.github.io/personal-businessapps/
- **Stack**: Single HTML page, no database, no frameworks
- **PWA**: Manifest + service worker for home screen install
- **Design**: Gradient header (teal to purple), 3-column tile grid
- **Cost**: Free (GitHub Pages hosting only)

## Sections & Apps

### Personal Hubs
| App | URL | Icon |
|-----|-----|------|
| Baker Hub | cathcoach4u.github.io/personal-baker-hub/ | Teal B |
| Cath Hub | cathcoach4u.github.io/personal-cath-hub/ | Teal C |
| Baker AI | cathcoach4u.github.io/personal-baker-hub/ai.html | Purple B |
| Cath AI | cathcoach4u.github.io/personal-cath-hub/ai.html | Purple C |
| Morning | cathcoach4u.github.io/personal-cath-hub/morning.html | Yellow sun |
| AisleMate | cathcoach4u.github.io/personal-baker-hub/shopping.html | Blue Sh |

### Coach4U — Clients
| App | URL | Icon |
|-----|-----|------|
| IAS | cathcoach4u.github.io/client_IAS/ | Red I |

### Coach4U — Internal
| App | URL | Icon |
|-----|-----|------|
| Coach4U Hub | cathcoach4u.github.io/internal-coach4u-hub/ | Dark blue C4U |
| C4U Bot | cathcoach4u.github.io/internal-coach4u-hub/bot.html | Chat bubble C4U |
| Coach4U Hub (old) | coach4u.com.au/appspersonalprofessional/coach4uhub/ | Dimmed C4U |
| Professional Dev | cathcoach4u.github.io/Internal-Resources-Training/ | Dark blue P |

### Coach4U — External
| App | URL | Icon |
|-----|-----|------|
| Resources | cathcoach4u.github.io/external-Coach4U-resources/ | Dark blue R |
| ThriveHQ | linktr.ee/thrivehq | Dark blue TH |

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
| index.html | The apps page (main entry point) |
| manifest.json | PWA manifest |
| sw.js | Service worker for offline/caching |
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
