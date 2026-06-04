---
name: gogolook-slides
description: Gogolook presentation design system — slide templates, layout patterns, data visualization, and typography rules for creating brand-compliant presentations. Use when building pitch decks, investor presentations, internal all-hands slides, conference talks, partner decks, or any Gogolook-branded slide content. Also use when reviewing existing presentations for brand compliance.
---

# Gogolook Presentation Design System

You are creating or reviewing a **Gogolook-branded presentation**. Every slide must reinforce the Gogolook identity: confident, clear, and visually grounded in the brand color system. This skill is self-contained; all rules are inline.

## Quick Reference

- **Primary color:** `#0058EA` (Gogolook Blue — dominant, ~50% at deck level)
- **Dark anchor:** `#0F2647` (Shadow Blue — ~20%)
- **Secondary accent:** `#00C0FE` (Clear Horizon — ~20%)
- **Highlight accent:** `#01D3B8` (Neo Green — ~10%, sparingly for data accents + CTAs)
- **Title font:** Plus Jakarta Sans Bold
- **Body font:** Inter Regular / Medium
- **Body text color:** `#000000` on light, `#FFFFFF` on dark
- **One idea per slide.** If it needs two takeaways, it needs two slides.

## Slide Dimensions and Safe Zones

### Standard Dimensions

| Format | Width | Height | Aspect Ratio |
|---|---|---|---|
| **Widescreen (default)** | 1920px | 1080px | 16:9 |
| **Keynote standard** | 1024px | 768px | 4:3 (avoid if possible) |

### Safe Zones

- **Title safe:** 80px inset from all edges (1920x1080) or 5% of canvas
- **Action safe:** 48px inset from all edges (1920x1080) or 2.5% of canvas
- No text, logos, or critical elements outside the title-safe zone
- Decorative elements (gradients, Concentric Effects) may bleed to the action-safe boundary

## Color Proportion at Deck Level

The 50/20/20/10 ratio applies across the **entire deck**, not to every individual slide:

- **~50% of slide area** across the deck should feature Gogolook Blue (backgrounds, headers, hero panels)
- **~20% Shadow Blue** — dark slides, section dividers, footer bars
- **~20% Clear Horizon** — accent panels, chart elements, supporting graphics
- **~10% Neo Green** — data highlights, key metrics, success indicators

This means some slides will be predominantly Blue while others use Shadow Blue or White. The mix should feel balanced when flipping through the deck.

## Typography for Slides

### Heading Hierarchy

| Level | Font | Weight | Size (1920x1080) | Line Height | Usage |
|---|---|---|---|---|---|
| Slide title | Plus Jakarta Sans | Bold (700) | 48-64px | 110% | Main slide headline |
| Subtitle | Plus Jakarta Sans | SemiBold (600) | 28-36px | 120% | Supporting headline |
| Section label | Plus Jakarta Sans | Bold (700) | 18-24px | 140% | Category / section name above title |

### Body Text

| Style | Font | Weight | Size (1920x1080) | Line Height | Usage |
|---|---|---|---|---|---|
| Body | Inter | Regular (400) | 20-24px | 150% | Bullet points, descriptions |
| Body emphasis | Inter | Medium (500) | 20-24px | 150% | Key phrases within body |
| Caption | Inter | Regular (400) | 14-16px | 140% | Source citations, footnotes |
| Data label | Inter | Medium (500) | 16-20px | 120% | Chart labels, KPI units |
| KPI number | Plus Jakarta Sans | Bold (700) | 64-96px | 100% | Hero data points |

### Rules

- Maximum two font sizes per slide (title + body). A third size is allowed only for captions or labels.
- Left-align all text. Center alignment only on title/cover slides.
- Never use more than 6 bullet points per slide.
- Each bullet should be one line (two lines maximum). If bullets wrap to three lines, split the slide.

## Slide Templates

### 1. Cover Slide

**Purpose:** First slide. Sets the tone.

**Layout:**
- Background: soft gradient from `#0058EA` to `#0F2647` (135-degree angle) or solid Gogolook Blue
- Title: White, Plus Jakarta Sans Bold, 56-64px, centered or left-aligned in the lower third
- Subtitle: White at 80% opacity, Inter Regular, 24px, directly below title
- Gogolook wordmark: White, bottom-right corner or bottom-center, within safe zone
- Optional: one Concentric Effect in the upper-right quadrant

**CSS gradient for cover:**
```css
background: linear-gradient(135deg, #0058EA 0%, #0F2647 100%);
```

### 2. Agenda Slide

**Purpose:** Outline the deck structure.

**Layout:**
- Background: White
- Title: "Agenda" in Gogolook Blue, top-left
- Items: numbered list, Inter Medium 24px, Black text
- Active/current item can be highlighted with Gogolook Blue text and a Blue left-border bar (4px)
- Optional: thin Blue horizontal rule below the title

### 3. Section Divider

**Purpose:** Separates major sections within the deck.

**Layout options:**
- **Option A (Dark):** Solid Shadow Blue `#0F2647` background. Section number in Neo Green `#01D3B8` (64px, Bold). Section title in White (48px, Bold). Centered vertically, left-aligned horizontally.
- **Option B (Blue):** Solid Gogolook Blue `#0058EA` background. Section title in White (48px, Bold), centered. Optional Concentric Effect, bottom-left.
- **Option C (White):** White background. Large section number in Blue (120px, Bold, 10% opacity). Section title overlaid in Shadow Blue (48px, Bold).

### 4. Content Slide (Text + Visual)

**Purpose:** Standard workhorse slide for presenting information.

**Layout:**
- Background: White
- Title: Gogolook Blue or Shadow Blue, Plus Jakarta Sans Bold, 36-48px, top-left
- Body text: Black, Inter Regular, 20-24px
- Split layout options:
  - **60/40:** Text left (60%), image or graphic right (40%)
  - **50/50:** Equal halves
  - **Full-width:** Text above, visual below (or visual as background with text overlay panel)
- Accent bar: 4px Gogolook Blue vertical bar left of the title, or horizontal bar below it
- Footer: slide number in Dark Grey, bottom-right, Inter Regular 14px

### 5. Data / Chart Slide

**Purpose:** Presenting metrics, charts, and quantitative information.

**Layout:**
- Background: White or Light Grey `#F5F7FA`
- Chart occupies 60-70% of the slide area
- Title: top-left, Gogolook Blue
- Source citation: bottom-left, Inter Regular 14px, Dark Grey
- Key insight callout: one sentence in Plus Jakarta Sans SemiBold 24px, positioned near the relevant data point

### 6. Quote Slide

**Purpose:** Highlight a testimonial, customer quote, or key statement.

**Layout:**
- Background: Shadow Blue `#0F2647` or Gogolook Blue `#0058EA`
- Large opening quotation mark: Neo Green `#01D3B8`, 120px, decorative
- Quote text: White, Inter Regular 28-32px, max 3 lines
- Attribution: White at 60% opacity, Inter Regular 18px, below quote
- Optional: small headshot (circle-cropped, 80px) left of attribution

### 7. Closing Slide

**Purpose:** Final slide. Call to action or thank you.

**Layout:**
- Background: same gradient as cover, or solid Gogolook Blue
- Message: White, Plus Jakarta Sans Bold, 48px ("Thank You" / "Let's Talk" / CTA)
- Contact info or URL: White at 80% opacity, Inter Regular 20px
- Gogolook wordmark: White, centered, below contact info
- Optional: Concentric Effect, subtle, in corners

## Data Visualization

### Color Assignment for Charts

Assign chart colors in this priority order:

1. **Primary data series:** Gogolook Blue `#0058EA`
2. **Secondary series:** Clear Horizon `#00C0FE`
3. **Tertiary series:** Shadow Blue `#0F2647`
4. **Highlight / callout:** Neo Green `#01D3B8`
5. **Additional series (if needed):** Use tint variants — `#80ABF5`, `#80DFFF`, `#8793A3`

### Chart Rules

- **Bar charts:** Gogolook Blue for primary, tints for secondary. Highlight bar in Neo Green for the key data point.
- **Line charts:** Gogolook Blue for primary line (2-3px stroke). Additional lines use Clear Horizon and Shadow Blue. Never more than 4 lines.
- **Pie / donut charts:** Maximum 5 segments. Use the brand palette in proportion order. Label each segment directly (no legends if possible).
- **KPI cards:** Large number in Gogolook Blue or Neo Green (Plus Jakarta Sans Bold 64-96px). Label in Inter Regular 16px. Up/down indicator arrow in Neo Green (up) or `#E53E3E` (down, non-brand red for clarity).
- **Gridlines:** Light Grey `#E2E8F0` at 1px. Never black gridlines.
- **Axis labels:** Inter Regular 14px, Dark Grey `#4A5568`.

### Data Slide Don'ts

- Never use 3D chart effects.
- Never use chart borders or boxes around the chart area.
- Never present data without a clear title stating the insight.
- Never use more than 5 colors in a single chart.

## Concentric Effect (Decoration)

### On Slides

- Maximum **one** Concentric Effect per slide
- 3-4 concentric ring outlines
- Stroke weight: 0.5pt-1pt
- Color: White at 10-25% opacity on colored/dark backgrounds; Gogolook Blue at 10-25% opacity on white backgrounds
- Position in a corner or along an edge; never centered on a slide (it would compete with content)
- Rings must not overlap with any text, data, or the logo
- Best used on: cover slides, section dividers, and closing slides
- Avoid on: data-heavy slides, text-heavy content slides

## Animations and Transitions

### Slide Transitions

- **Default:** Simple fade or cut. No wipes, spins, or 3D transitions.
- **Duration:** 300-500ms maximum
- Use the same transition throughout the deck for consistency

### Element Animations

- **Entrance:** Fade-in or slide-up. No bounce, zoom, or fly-in.
- **Build:** Bullet points appear one at a time via fade (not typewriter).
- **Charts:** Bars or lines animate from zero to value (if the tool supports it).
- **Duration:** 200-400ms per element

### Rules

- Never auto-advance slides.
- Never use sound effects.
- Limit animations to one build per slide. Over-animated decks feel unprofessional.

## Deck Structure Template

A standard Gogolook presentation follows this skeleton. Adapt as needed, but maintain the rhythm of content-to-divider-to-content.

```
1. Cover (gradient or solid Blue)
2. Agenda
3. Section Divider — Context
4. Content slide(s) — background, problem, opportunity
5. Section Divider — Solution
6. Content slide(s) — product, features, demo
7. Section Divider — Traction / Data
8. Data slide(s) — KPIs, charts, growth
9. Quote slide — testimonial or key insight
10. Section Divider — Next Steps
11. Content slide(s) — roadmap, ask, timeline
12. Closing (gradient or solid Blue)
```

## Output Checklist

Before delivering any Gogolook presentation, verify:

- [ ] **Dimensions** are 1920x1080 (16:9) unless specifically requested otherwise
- [ ] **Color proportions** approximate 50/20/20/10 across the full deck
- [ ] **Title slides** use Gogolook Blue on White or White on Blue/Shadow Blue
- [ ] **Cover background** uses the `#0058EA` to `#0F2647` gradient or solid Blue
- [ ] **Fonts** are Plus Jakarta Sans Bold for titles, Inter for body
- [ ] **One idea per slide** — no slide tries to communicate two separate concepts
- [ ] **Max 6 bullets** per slide; each bullet fits in 1-2 lines
- [ ] **Charts** use brand colors in priority order; no 3D effects or chart boxes
- [ ] **Concentric Effect** appears at most once per slide, 3-4 rings, 0.5-1pt stroke
- [ ] **Transitions** are simple fades or cuts, consistent throughout
- [ ] **Logo** appears on cover and closing slides with correct clear space
- [ ] **Text contrast** meets readability standards on every slide
- [ ] **Slide numbers** appear on content slides (not on cover or closing)
