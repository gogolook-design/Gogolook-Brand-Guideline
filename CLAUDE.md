# Gogolook Brand Design Guidelines V1

## Global Memory

Read ~/.claude/CLAUDE.md for memory rules and topic files.

## Project Overview

Single-page static website presenting the Gogolook Brand Design Guidelines. The site is password-protected and deployed to GitHub Pages under the `gogolook-design` organization. It contains seven chapters covering logo, colors, typography, layout, photography, gradients, and downloadable AI skills.

## Tech Stack

- Plain HTML + inline CSS (no build tools, no npm, no frameworks)
- Google Fonts CDN for web fonts
- Client-side JavaScript for password gate and navigation
- Deployed via GitHub Pages on the `main` branch

## File Structure

```
/
├── CLAUDE.md              # This file
├── README.md              # Project readme
├── index.html             # Single-page brand guideline (all chapters)
├── assets/
│   ├── logo/              # SVG logos, usage PNGs, historical logos, incorrect-use examples
│   ├── colors/            # Color swatches, gradients, usage proportions
│   ├── layout/            # Grid systems (2/3/6-col), margin guides
│   └── photography/       # Photography style examples (lifestyle, environment, connected)
└── skills/                # Downloadable Claude Code SKILL.md files
    ├── gogolook-brand-SKILL.md
    ├── gogolook-slides-SKILL.md
    └── gogolook-ui-SKILL.md
```

## Brand Tokens Quick Reference

### Colors

| Name            | Hex       | Role                        |
|-----------------|-----------|-----------------------------|
| Gogolook Blue   | `#0058EA` | Primary brand color         |
| Neo Green       | `#01D3B8` | Accent / highlight          |
| Shadow Blue     | `#0F2647` | Dark backgrounds, sidebar   |
| Clear Horizon   | `#00C0FE` | Supporting blue             |
| Genuine Blue    | `#008CF4` | Supporting blue             |
| Intelligent Blue| `#D0E3FC` | Light blue for backgrounds  |

### Color Proportions

- 50% Gogolook Blue (`#0058EA`)
- 20% Shadow Blue (`#0F2647`)
- 20% Clear Horizon (`#00C0FE`)
- 10% Neo Green (`#01D3B8`)

### Typography

| Usage    | Font Family       | Source           |
|----------|-------------------|------------------|
| Headings | Plus Jakarta Sans | Google Fonts CDN |
| Body     | Inter             | Google Fonts CDN |
| CJK      | Noto Sans         | Google Fonts CDN |

### Gradients

- Standard gradient: Gogolook Blue to Clear Horizon (135deg)
- Duotone, freeform, and alternative gradient variants documented in Chapter 06

## Password Gate

Client-side JavaScript password protection. The gate overlay appears on page load and hides the content until a valid password is entered.

**Accepted passwords:** `gogolook2026`, `1234`

This is a lightweight deterrent, not secure authentication. All content is in the HTML source.

## Chapters

1. **Logo** — Evolution (2012-2024), preferred usage, monochrome variants, incorrect usage
2. **Colors** — Primary palette, supporting colors, usage proportions
3. **Typography** — Font families, weights, sizing scale
4. **Layout** — Grid systems (2/3/6-column), margin rules (landscape/portrait/square)
5. **Photography** — Style direction (lifestyle, environment, connected), do/don't examples
6. **Gradient** — Standard, duotone, freeform variants, usage guidelines
7. **AI Skills** — Three downloadable SKILL.md files for Claude Code

## Deployment

1. Push changes to the `main` branch of `gogolook-design/Gogolook_brand_guideline` on GitHub
2. GitHub Pages serves from the root of `main`
3. No build step required — the site is the raw HTML file

## Constraints

- No build step, no npm, no package.json
- All CSS is inline in `index.html` (no external stylesheets)
- Fonts loaded from Google Fonts CDN only
- Images in `assets/` are referenced with relative paths
- Keep the site as a single `index.html` file
- Skill files in `skills/` are plain Markdown, downloaded via JS blob links
