---
name: gogolook-brand
description: Gogolook corporate brand identity — visual identity, voice, color, typography, logo, photography, layout, and gradient rules. Use when generating any Gogolook parent-brand content: corporate website, investor materials, press kits, social posts, event collateral, internal templates, or partner-facing assets. Also use when reviewing existing Gogolook assets for brand compliance.
---

# Gogolook Corporate Brand Identity

You are working on brand assets for **Gogolook** — the parent company behind Whoscall, ScamAdviser, and other trust-technology products. Every output must reflect the Gogolook corporate identity: confident, forward-looking, and grounded in the mission of building trust in communication. This skill is self-contained; all rules are inline.

## Quick Reference

- **Primary color:** `#0058EA` (Gogolook Blue — ~50% of composition, dominant brand surface)
- **Accent color:** `#01D3B8` (Neo Green — ~10%, highlights + CTAs + data accents)
- **Dark anchor:** `#0F2647` (Shadow Blue — ~20%, dark backgrounds + text on light surfaces)
- **Secondary accent:** `#00C0FE` (Clear Horizon — ~20%, supporting UI + illustrations)
- **Heading font:** Plus Jakarta Sans Bold
- **Body font:** Inter Regular
- **Body text color:** `#000000` (Black)
- **Brand feeling:** Clear, Relatable, Empowering
- **Tone:** Confident but approachable, professional without being cold, optimistic without being naive
- **Never:** Fear-based messaging, judgmental language, overly technical jargon, condescending tone

## Color System

### Primary Palette

| Role | Name | Hex | Proportion |
|---|---|---|---|
| **Primary** | Gogolook Blue | `#0058EA` | ~50% |
| **Dark anchor** | Shadow Blue | `#0F2647` | ~20% |
| **Secondary accent** | Clear Horizon | `#00C0FE` | ~20% |
| **Highlight accent** | Neo Green | `#01D3B8` | ~10% |

### Color Proportion Rule

The 50/20/20/10 ratio governs overall composition across any deliverable:

- **50% Gogolook Blue** — the dominant brand signal. Backgrounds, headers, hero panels.
- **20% Shadow Blue** — anchoring depth. Dark sections, footer, overlays, body text on light backgrounds.
- **20% Clear Horizon** — supporting energy. Secondary panels, illustrations, icon fills.
- **10% Neo Green** — sparingly deployed for maximum impact. CTAs, success states, data highlights, badges.

### Tint Scale

Each primary color has tint variants for subtle UI needs:

| Base | Tint-01 (80%) | Tint-02 (50%) | Tint-03 (20%) |
|---|---|---|---|
| `#0058EA` | `#3379EE` | `#80ABF5` | `#CCDDFA` |
| `#0F2647` | `#3F516C` | `#8793A3` | `#CFD4DB` |
| `#00C0FE` | `#33CDFE` | `#80DFFF` | `#CCF2FF` |
| `#01D3B8` | `#34DCC6` | `#80E9DB` | `#CCF5EF` |

### Neutrals

| Name | Hex | Usage |
|---|---|---|
| White | `#FFFFFF` | Page backgrounds, cards, text on dark |
| Light Grey | `#F5F7FA` | Subtle background panels |
| Mid Grey | `#C4C9D2` | Borders, dividers |
| Dark Grey | `#4A5568` | Secondary text |
| Black | `#000000` | Body text on light backgrounds |

## Gradient

### Standard 4-Color Gradient

A smooth blend of all four brand colors, used for hero backgrounds, feature highlights, and digital brand moments.

**Stops:** `#0058EA` -> `#00C0FE` -> `#01D3B8` -> `#0F2647`

**CSS:**
```css
background: linear-gradient(135deg, #0058EA 0%, #00C0FE 35%, #01D3B8 65%, #0F2647 100%);
```

### Rules

- **Digital only.** Never reproduce the gradient in print.
- Apply as background fills, overlay washes, or border accents.
- Maintain smooth transitions; do not posterize or band.
- Always ensure text over gradient meets WCAG AA contrast (use white text or a semi-transparent dark overlay).

### Alternative Gradients

**Duotone (Blue to Shadow):**
```css
background: linear-gradient(135deg, #0058EA 0%, #0F2647 100%);
```

**Freeform:** For creative/editorial contexts, the four brand colors may be arranged in freeform gradient blobs. Keep it organic, never harsh.

## Typography

### Heading Stack

| Level | Font | Weight | Size | Line Height | Usage |
|---|---|---|---|---|---|
| H1 | Plus Jakarta Sans | Bold (700) | 40px | 100% (1.0) | Page titles, hero headlines |
| H2 | Plus Jakarta Sans | Bold (700) | 18px | 140% (1.4) | Section headings |
| H3 | Plus Jakarta Sans | SemiBold (600) | 16px | 140% (1.4) | Subsection headings |
| H4 | Plus Jakarta Sans | SemiBold (600) | 14px | 140% (1.4) | Card titles, labels |

### Body Stack

| Style | Font | Weight | Size | Line Height | Usage |
|---|---|---|---|---|---|
| Body | Inter | Regular (400) | 16px | 160% (1.6) | Paragraphs, descriptions |
| Body Small | Inter | Regular (400) | 14px | 160% (1.6) | Captions, metadata |
| Label | Inter | Medium (500) | 12px | 140% (1.4) | UI labels, tags |

### Rules

- Headings use **Plus Jakarta Sans Bold** exclusively. Never substitute with Inter for headings.
- Body text uses **Inter Regular**. Use Inter Medium (500) sparingly for emphasis within body text.
- Body text color is always `#000000` (Black) on light backgrounds, `#FFFFFF` (White) on dark backgrounds.
- Never use more than two font sizes on a single card or module.
- Google Fonts links: [Plus Jakarta Sans](https://fonts.google.com/specimen/Plus+Jakarta+Sans), [Inter](https://fonts.google.com/specimen/Inter).

## Logo

### Primary Logo

The Gogolook logo is a **wordmark** only (no symbol or icon). The custom letterforms are the full identity.

### Preferred Treatments

| Context | Logo Color | Background |
|---|---|---|
| **Preferred (light)** | Gogolook Blue `#0058EA` | White `#FFFFFF` |
| **Preferred (dark)** | White `#FFFFFF` | Gogolook Blue `#0058EA` |
| **Monochrome light** | White `#FFFFFF` | Dark backgrounds (Shadow Blue, Black) |
| **Monochrome dark** | Black `#000000` | White or very light backgrounds |

### Clear Space

The minimum clear space around the wordmark equals the **height of the capital G** in the wordmark, measured on all four sides. No other element (text, icon, border, pattern) may enter this zone.

### Minimum Size

- **Web / digital:** 100px minimum width
- **Print:** 25mm minimum width

### Incorrect Usage (Never Do)

1. Do not rotate or skew the wordmark.
2. Do not alter letter spacing or proportions.
3. Do not place the wordmark over busy or low-contrast imagery without a backing panel.
4. Do not add shadows, outlines, or effects.
5. Do not crop or partially obscure the wordmark.
6. Do not recolor the wordmark in non-brand colors.

## Voice and Tone

### Brand Voice Attributes

1. **Clear** — Straightforward language. No jargon unless the audience is technical. If a 15-year-old cannot understand it, rewrite.
2. **Relatable** — Warm and human. Gogolook solves a problem everyone faces. Speak like a knowledgeable friend, not a corporation.
3. **Empowering** — Give people the tools and confidence to protect themselves. Frame the user as the hero, Gogolook as the enabler.

### Writing Rules

- Lead with benefit, not feature.
- Active voice always. Passive voice only when the actor is genuinely unknown.
- Short paragraphs (3 sentences max per paragraph in marketing copy).
- Never use fear-based language ("You WILL be scammed if...").
- Never be judgmental toward people who fall for scams.
- Avoid superlatives ("the best," "the only") unless backed by a specific data point.
- Use "we" for Gogolook. Use "you" for the audience. Never "one" or "users."

### Example Translations

| Before (wrong) | After (right) |
|---|---|
| "Our AI-powered engine leverages ML to detect fraud vectors." | "We catch scam calls so you don't have to." |
| "Users must exercise caution when receiving unknown calls." | "Got a weird call? We'll tell you who it is." |
| "Gogolook is the #1 leader in caller ID." | "850 million calls identified and counting." |

## Photography

### Style Direction

All Gogolook photography follows an editorial, lifestyle-first approach:

- **Lighting:** Bright, natural light. Prefer golden hour or soft indirect daylight. Never harsh flash.
- **Saturation:** High but natural. Colors should feel vivid and optimistic, not over-processed.
- **Mood:** Candid over posed. Capture real moments of connection, work, and daily life.
- **Subjects:** Diverse people in authentic settings. Technology is present but never the hero; people are.
- **Composition:** Editorial style — asymmetric crops, environmental context, shallow depth of field for portraits.

### Categories

1. **Connected life** — People using phones, laptops, or tech in natural daily contexts.
2. **Lifestyle** — Moments of joy, trust, community. No stock-photo smiles.
3. **Environment** — Workspaces, cities, nature. Context that grounds the brand in the real world.

### Do Not

- Use obviously staged stock photography.
- Show isolated devices on white backgrounds (product shots are not brand photography).
- Use dark, moody, or threatening imagery.
- Show people looking frightened, victimized, or distressed.

## Layout

### Grid System

- **Standard grid:** 12 columns
- **Gutter width:** 24px (desktop), 16px (mobile)
- **Common column spans:** 12 (full), 6 (half), 4 (third), 3 (quarter)

### Diagonal Margin

A signature Gogolook layout device: angled crop lines or diagonal panel edges that create dynamic energy.

- **Minimum diagonal margin:** 6% of the shorter dimension of the canvas
- Use diagonals to separate content sections or as decorative panel edges
- Never let diagonals interfere with text readability or logo clear space

### Spacing Scale

Use these values for padding, margins, and gaps:

`4 | 8 | 12 | 16 | 20 | 24 | 32 | 40 | 48 | 64 | 80 | 96 | 120` (px)

### Container Widths

| Breakpoint | Max Content Width |
|---|---|
| Mobile (< 768px) | 100% with 16px side padding |
| Tablet (768-1023px) | 720px |
| Desktop (1024-1439px) | 960px |
| Wide (>= 1440px) | 1200px |

## Concentric Effect

A brand-specific decorative motif: concentric ring outlines radiating from a focal point.

### Rules

- 3-4 ring outlines per instance
- Stroke weight: 0.5pt-1pt
- Color: White at 10-25% opacity (on dark/colored backgrounds) or Gogolook Blue at 10-25% opacity (on white)
- Maximum one Concentric Effect per layout section
- Rings should not overlap with text or logos
- Use to draw the eye to a key element or to fill empty space in asymmetric compositions

## Output Checklist

Before delivering any Gogolook brand asset, verify:

- [ ] **Color proportions** follow 50/20/20/10 (Blue / Shadow / Horizon / Green)
- [ ] **Heading font** is Plus Jakarta Sans Bold
- [ ] **Body font** is Inter Regular; body text color is Black (#000000) on light or White on dark
- [ ] **Logo** uses an approved color treatment with correct clear space
- [ ] **Logo** meets minimum size (100px web, 25mm print)
- [ ] **Voice** is Clear, Relatable, Empowering — no fear-based or judgmental language
- [ ] **Photography** (if used) is bright, natural light, candid, editorial
- [ ] **Gradient** (if used) is digital-only, 4-color standard or approved alternative
- [ ] **Layout** uses 12-column grid with correct spacing scale
- [ ] **Diagonal margins** (if used) are at least 6% of the shorter canvas dimension
- [ ] **Concentric Effect** (if used) has 3-4 rings, 0.5-1pt stroke, max one per section
- [ ] **Contrast** meets WCAG AA for all text on background combinations
- [ ] **Tone** avoids superlatives, passive voice, jargon, and fear-based framing
