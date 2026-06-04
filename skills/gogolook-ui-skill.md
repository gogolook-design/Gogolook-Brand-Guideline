---
name: gogolook-ui
description: Gogolook web design system — CSS tokens, component patterns, layout rules, typography, color scales, animations, dark mode, gradients, and accessibility requirements for building Gogolook-style web interfaces. Use when building web pages, UI components, landing pages, dashboards, or any coded interface that must follow the Gogolook visual identity. Also use when reviewing web implementations against the design system.
---

# Gogolook Web Design System

You are building or reviewing a **Gogolook-branded web interface**. This skill provides the complete design token system, component patterns, and layout rules needed to produce production-grade, brand-compliant web UI. This skill is self-contained; all tokens and patterns are inline.

## Quick Reference

- **Primary:** `#0058EA` (Gogolook Blue), **Dark:** `#0F2647` (Shadow Blue), **Accent:** `#00C0FE` (Clear Horizon), **Highlight:** `#01D3B8` (Neo Green)
- **Heading font:** Plus Jakarta Sans Bold | **Body font:** Inter Regular
- **Grid:** 12 columns | **Max width:** 1200px | **Base unit:** 4px
- **Border radius:** 8px default | **Transition:** 200ms ease
- **Breakpoints:** 375 / 768 / 1024 / 1440

---

## CSS Custom Properties (Copy-Paste Ready)

```css
:root {
  /* ========================================
     GOGOLOOK DESIGN TOKENS
     ======================================== */

  /* --- Brand Colors --- */
  --gl-blue:            #0058EA;
  --gl-blue-01:         #3379EE;
  --gl-blue-02:         #80ABF5;
  --gl-blue-03:         #CCDDFA;

  --gl-shadow:          #0F2647;
  --gl-shadow-01:       #3F516C;
  --gl-shadow-02:       #8793A3;
  --gl-shadow-03:       #CFD4DB;

  --gl-horizon:         #00C0FE;
  --gl-horizon-01:      #33CDFE;
  --gl-horizon-02:      #80DFFF;
  --gl-horizon-03:      #CCF2FF;

  --gl-green:           #01D3B8;
  --gl-green-01:        #34DCC6;
  --gl-green-02:        #80E9DB;
  --gl-green-03:        #CCF5EF;

  /* --- Neutrals --- */
  --gl-white:           #FFFFFF;
  --gl-gray-50:         #F9FAFB;
  --gl-gray-100:        #F5F7FA;
  --gl-gray-200:        #E2E8F0;
  --gl-gray-300:        #C4C9D2;
  --gl-gray-400:        #94A3B8;
  --gl-gray-500:        #64748B;
  --gl-gray-600:        #4A5568;
  --gl-gray-700:        #334155;
  --gl-gray-800:        #1E293B;
  --gl-gray-900:        #0F172A;
  --gl-black:           #000000;

  /* --- Semantic Colors --- */
  --gl-success:         #01D3B8;
  --gl-success-bg:      #CCF5EF;
  --gl-warning:         #F59E0B;
  --gl-warning-bg:      #FEF3C7;
  --gl-error:           #EF4444;
  --gl-error-bg:        #FEE2E2;
  --gl-info:            #00C0FE;
  --gl-info-bg:         #CCF2FF;

  /* --- Typography --- */
  --gl-font-heading:    'Plus Jakarta Sans', 'Inter', system-ui, sans-serif;
  --gl-font-body:       'Inter', system-ui, -apple-system, sans-serif;
  --gl-font-mono:       'JetBrains Mono', 'Fira Code', monospace;

  /* Font sizes */
  --gl-text-xs:         12px;
  --gl-text-sm:         14px;
  --gl-text-base:       16px;
  --gl-text-lg:         18px;
  --gl-text-xl:         20px;
  --gl-text-2xl:        24px;
  --gl-text-3xl:        30px;
  --gl-text-4xl:        36px;
  --gl-text-5xl:        40px;
  --gl-text-6xl:        48px;
  --gl-text-7xl:        64px;

  /* Font weights */
  --gl-weight-regular:  400;
  --gl-weight-medium:   500;
  --gl-weight-semibold: 600;
  --gl-weight-bold:     700;

  /* Line heights */
  --gl-leading-none:    1.0;
  --gl-leading-tight:   1.2;
  --gl-leading-snug:    1.4;
  --gl-leading-normal:  1.6;
  --gl-leading-relaxed: 1.75;

  /* --- Spacing Scale --- */
  --gl-space-1:         4px;
  --gl-space-2:         8px;
  --gl-space-3:         12px;
  --gl-space-4:         16px;
  --gl-space-5:         20px;
  --gl-space-6:         24px;
  --gl-space-8:         32px;
  --gl-space-10:        40px;
  --gl-space-12:        48px;
  --gl-space-16:        64px;
  --gl-space-20:        80px;
  --gl-space-24:        96px;
  --gl-space-30:        120px;

  /* --- Border Radius --- */
  --gl-radius-sm:       4px;
  --gl-radius-md:       8px;
  --gl-radius-lg:       12px;
  --gl-radius-xl:       16px;
  --gl-radius-2xl:      20px;
  --gl-radius-3xl:      24px;
  --gl-radius-full:     9999px;

  /* --- Shadows --- */
  --gl-shadow-sm:       0 1px 2px rgba(15, 38, 71, 0.05);
  --gl-shadow-md:       0 4px 6px -1px rgba(15, 38, 71, 0.07), 0 2px 4px -2px rgba(15, 38, 71, 0.05);
  --gl-shadow-lg:       0 10px 15px -3px rgba(15, 38, 71, 0.08), 0 4px 6px -4px rgba(15, 38, 71, 0.04);
  --gl-shadow-xl:       0 20px 25px -5px rgba(15, 38, 71, 0.10), 0 8px 10px -6px rgba(15, 38, 71, 0.05);

  /* --- Transitions --- */
  --gl-transition-fast:    150ms ease;
  --gl-transition-base:    200ms ease;
  --gl-transition-slow:    300ms ease;
  --gl-transition-page:    300ms ease-in-out;

  /* --- Breakpoints (for reference; use in media queries) --- */
  /* Mobile:  375px  */
  /* Tablet:  768px  */
  /* Desktop: 1024px */
  /* Wide:    1440px */

  /* --- Layout --- */
  --gl-container-sm:    640px;
  --gl-container-md:    768px;
  --gl-container-lg:    960px;
  --gl-container-xl:    1200px;
  --gl-grid-columns:    12;
  --gl-grid-gutter:     24px;

  /* --- Gradients --- */
  --gl-gradient-standard:  linear-gradient(135deg, #0058EA 0%, #00C0FE 35%, #01D3B8 65%, #0F2647 100%);
  --gl-gradient-duotone:   linear-gradient(135deg, #0058EA 0%, #0F2647 100%);
  --gl-gradient-blue:      linear-gradient(135deg, #0058EA 0%, #00C0FE 100%);
  --gl-gradient-fresh:     linear-gradient(135deg, #00C0FE 0%, #01D3B8 100%);
  --gl-gradient-dark:      linear-gradient(135deg, #0F2647 0%, #0058EA 100%);
}
```

---

## Dark Mode Tokens

```css
[data-theme="dark"],
.gl-dark {
  /* --- Surfaces --- */
  --gl-bg-primary:      #0F2647;
  --gl-bg-secondary:    #162D52;
  --gl-bg-tertiary:     #1C3660;
  --gl-bg-elevated:     #22406E;

  /* --- Text --- */
  --gl-text-primary:    #FFFFFF;
  --gl-text-secondary:  rgba(255, 255, 255, 0.72);
  --gl-text-tertiary:   rgba(255, 255, 255, 0.48);
  --gl-text-disabled:   rgba(255, 255, 255, 0.24);

  /* --- Borders --- */
  --gl-border-default:  rgba(255, 255, 255, 0.12);
  --gl-border-subtle:   rgba(255, 255, 255, 0.06);
  --gl-border-emphasis: rgba(255, 255, 255, 0.24);

  /* --- Semantic (dark mode adjustments) --- */
  --gl-success:         #34DCC6;
  --gl-success-bg:      rgba(1, 211, 184, 0.15);
  --gl-warning:         #FBBF24;
  --gl-warning-bg:      rgba(245, 158, 11, 0.15);
  --gl-error:           #F87171;
  --gl-error-bg:        rgba(239, 68, 68, 0.15);
  --gl-info:            #33CDFE;
  --gl-info-bg:         rgba(0, 192, 254, 0.15);

  /* --- Shadows (deeper for dark surfaces) --- */
  --gl-shadow-sm:       0 1px 2px rgba(0, 0, 0, 0.20);
  --gl-shadow-md:       0 4px 6px -1px rgba(0, 0, 0, 0.30), 0 2px 4px -2px rgba(0, 0, 0, 0.20);
  --gl-shadow-lg:       0 10px 15px -3px rgba(0, 0, 0, 0.35), 0 4px 6px -4px rgba(0, 0, 0, 0.20);
  --gl-shadow-xl:       0 20px 25px -5px rgba(0, 0, 0, 0.40), 0 8px 10px -6px rgba(0, 0, 0, 0.25);
}
```

### Light Mode Tokens (default)

```css
:root {
  --gl-bg-primary:      #FFFFFF;
  --gl-bg-secondary:    #F5F7FA;
  --gl-bg-tertiary:     #E2E8F0;
  --gl-bg-elevated:     #FFFFFF;

  --gl-text-primary:    #000000;
  --gl-text-secondary:  #4A5568;
  --gl-text-tertiary:   #94A3B8;
  --gl-text-disabled:   #C4C9D2;

  --gl-border-default:  #E2E8F0;
  --gl-border-subtle:   #F5F7FA;
  --gl-border-emphasis: #C4C9D2;
}
```

---

## Typography

### Heading Styles

```css
.gl-h1 {
  font-family: var(--gl-font-heading);
  font-weight: var(--gl-weight-bold);
  font-size: var(--gl-text-5xl);      /* 40px */
  line-height: var(--gl-leading-none); /* 1.0 */
  letter-spacing: -0.02em;
  color: var(--gl-text-primary);
}

.gl-h2 {
  font-family: var(--gl-font-heading);
  font-weight: var(--gl-weight-bold);
  font-size: var(--gl-text-lg);       /* 18px */
  line-height: var(--gl-leading-snug); /* 1.4 */
  letter-spacing: -0.01em;
  color: var(--gl-text-primary);
}

.gl-h3 {
  font-family: var(--gl-font-heading);
  font-weight: var(--gl-weight-semibold);
  font-size: var(--gl-text-base);     /* 16px */
  line-height: var(--gl-leading-snug);
  color: var(--gl-text-primary);
}

.gl-h4 {
  font-family: var(--gl-font-heading);
  font-weight: var(--gl-weight-semibold);
  font-size: var(--gl-text-sm);       /* 14px */
  line-height: var(--gl-leading-snug);
  color: var(--gl-text-primary);
}
```

### Body Styles

```css
.gl-body {
  font-family: var(--gl-font-body);
  font-weight: var(--gl-weight-regular);
  font-size: var(--gl-text-base);      /* 16px */
  line-height: var(--gl-leading-normal); /* 1.6 */
  color: var(--gl-text-primary);
}

.gl-body-sm {
  font-family: var(--gl-font-body);
  font-weight: var(--gl-weight-regular);
  font-size: var(--gl-text-sm);        /* 14px */
  line-height: var(--gl-leading-normal);
  color: var(--gl-text-secondary);
}

.gl-label {
  font-family: var(--gl-font-body);
  font-weight: var(--gl-weight-medium);
  font-size: var(--gl-text-xs);        /* 12px */
  line-height: var(--gl-leading-snug);
  letter-spacing: 0.02em;
  text-transform: uppercase;
  color: var(--gl-text-tertiary);
}

.gl-caption {
  font-family: var(--gl-font-body);
  font-weight: var(--gl-weight-regular);
  font-size: var(--gl-text-xs);
  line-height: var(--gl-leading-snug);
  color: var(--gl-text-tertiary);
}
```

### Font Loading

```html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@600;700&family=Inter:wght@400;500;700&display=swap" rel="stylesheet">
```

---

## Layout System

### 12-Column Grid

```css
.gl-container {
  width: 100%;
  max-width: var(--gl-container-xl);  /* 1200px */
  margin: 0 auto;
  padding: 0 var(--gl-space-4);       /* 16px side padding */
}

@media (min-width: 768px) {
  .gl-container {
    padding: 0 var(--gl-space-6);     /* 24px */
  }
}

@media (min-width: 1024px) {
  .gl-container {
    padding: 0 var(--gl-space-8);     /* 32px */
  }
}

.gl-grid {
  display: grid;
  grid-template-columns: repeat(var(--gl-grid-columns), 1fr);
  gap: var(--gl-grid-gutter);         /* 24px */
}

@media (max-width: 767px) {
  .gl-grid {
    grid-template-columns: 1fr;
    gap: var(--gl-space-4);           /* 16px on mobile */
  }
}
```

### Column Utilities

```css
.gl-col-1  { grid-column: span 1; }
.gl-col-2  { grid-column: span 2; }
.gl-col-3  { grid-column: span 3; }
.gl-col-4  { grid-column: span 4; }
.gl-col-5  { grid-column: span 5; }
.gl-col-6  { grid-column: span 6; }
.gl-col-7  { grid-column: span 7; }
.gl-col-8  { grid-column: span 8; }
.gl-col-9  { grid-column: span 9; }
.gl-col-10 { grid-column: span 10; }
.gl-col-11 { grid-column: span 11; }
.gl-col-12 { grid-column: span 12; }

/* Responsive: stack on mobile, split on tablet+ */
@media (max-width: 767px) {
  [class*="gl-col-"] {
    grid-column: span 12;
  }
}
```

### Breakpoints Reference

| Name | Min Width | Typical Use |
|---|---|---|
| **Mobile** | 375px | Single column, stacked layout |
| **Tablet** | 768px | Two-column layouts, side navigation |
| **Desktop** | 1024px | Full 12-column grid, expanded navigation |
| **Wide** | 1440px | Max content width reached, centered |

### Spacing Rules

- Section padding (vertical): `--gl-space-20` (80px) desktop, `--gl-space-12` (48px) mobile
- Between components in a section: `--gl-space-10` (40px) desktop, `--gl-space-6` (24px) mobile
- Card internal padding: `--gl-space-6` (24px) desktop, `--gl-space-4` (16px) mobile
- Inline element gaps: `--gl-space-2` (8px) to `--gl-space-3` (12px)

---

## Component Patterns

### Buttons

```css
/* Base button */
.gl-btn {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  gap: var(--gl-space-2);
  padding: var(--gl-space-3) var(--gl-space-6);   /* 12px 24px */
  font-family: var(--gl-font-body);
  font-weight: var(--gl-weight-medium);
  font-size: var(--gl-text-sm);                    /* 14px */
  line-height: 1;
  border-radius: var(--gl-radius-md);              /* 8px */
  border: 1.5px solid transparent;
  cursor: pointer;
  transition: all var(--gl-transition-base);
  text-decoration: none;
  white-space: nowrap;
}

.gl-btn:focus-visible {
  outline: 2px solid var(--gl-blue);
  outline-offset: 2px;
}

/* Primary button */
.gl-btn-primary {
  background: var(--gl-blue);
  color: var(--gl-white);
  border-color: var(--gl-blue);
}

.gl-btn-primary:hover {
  background: var(--gl-blue-01);                   /* #3379EE */
  border-color: var(--gl-blue-01);
  box-shadow: var(--gl-shadow-md);
}

.gl-btn-primary:active {
  background: #0046BE;
  border-color: #0046BE;
}

/* Secondary button */
.gl-btn-secondary {
  background: var(--gl-white);
  color: var(--gl-blue);
  border-color: var(--gl-blue);
}

.gl-btn-secondary:hover {
  background: var(--gl-blue-03);                   /* #CCDDFA */
  border-color: var(--gl-blue);
}

.gl-btn-secondary:active {
  background: var(--gl-blue-02);
}

/* Ghost button */
.gl-btn-ghost {
  background: transparent;
  color: var(--gl-blue);
  border-color: transparent;
}

.gl-btn-ghost:hover {
  background: var(--gl-blue-03);
}

.gl-btn-ghost:active {
  background: var(--gl-blue-02);
}

/* Button sizes */
.gl-btn-sm {
  padding: var(--gl-space-2) var(--gl-space-4);    /* 8px 16px */
  font-size: var(--gl-text-xs);                    /* 12px */
  border-radius: var(--gl-radius-sm);
}

.gl-btn-lg {
  padding: var(--gl-space-4) var(--gl-space-8);    /* 16px 32px */
  font-size: var(--gl-text-base);                  /* 16px */
  border-radius: var(--gl-radius-lg);
}

/* Disabled state */
.gl-btn:disabled,
.gl-btn[aria-disabled="true"] {
  opacity: 0.4;
  cursor: not-allowed;
  pointer-events: none;
}
```

**Usage:**
```html
<button class="gl-btn gl-btn-primary">Get Started</button>
<button class="gl-btn gl-btn-secondary">Learn More</button>
<button class="gl-btn gl-btn-ghost">Cancel</button>
<button class="gl-btn gl-btn-primary gl-btn-lg">Download Now</button>
```

### Cards

```css
.gl-card {
  background: var(--gl-bg-elevated);
  border: 1px solid var(--gl-border-default);
  border-radius: var(--gl-radius-lg);              /* 12px */
  padding: var(--gl-space-6);                      /* 24px */
  box-shadow: var(--gl-shadow-sm);
  transition: box-shadow var(--gl-transition-base),
              transform var(--gl-transition-base);
}

.gl-card:hover {
  box-shadow: var(--gl-shadow-md);
  transform: translateY(-2px);
}

.gl-card-flat {
  box-shadow: none;
  border: 1px solid var(--gl-border-default);
}

.gl-card-flat:hover {
  box-shadow: none;
  transform: none;
  border-color: var(--gl-blue-02);
}

.gl-card-featured {
  border: 2px solid var(--gl-blue);
  box-shadow: var(--gl-shadow-md);
}

/* Card internal structure */
.gl-card__image {
  margin: calc(-1 * var(--gl-space-6));
  margin-bottom: var(--gl-space-4);
  border-radius: var(--gl-radius-lg) var(--gl-radius-lg) 0 0;
  overflow: hidden;
}

.gl-card__image img {
  width: 100%;
  height: auto;
  display: block;
}

.gl-card__title {
  font-family: var(--gl-font-heading);
  font-weight: var(--gl-weight-bold);
  font-size: var(--gl-text-lg);
  line-height: var(--gl-leading-snug);
  color: var(--gl-text-primary);
  margin-bottom: var(--gl-space-2);
}

.gl-card__body {
  font-family: var(--gl-font-body);
  font-size: var(--gl-text-sm);
  line-height: var(--gl-leading-normal);
  color: var(--gl-text-secondary);
}

.gl-card__footer {
  margin-top: var(--gl-space-4);
  padding-top: var(--gl-space-4);
  border-top: 1px solid var(--gl-border-subtle);
}
```

### Navigation Bar

```css
.gl-navbar {
  position: sticky;
  top: 0;
  z-index: 1000;
  display: flex;
  align-items: center;
  justify-content: space-between;
  height: 64px;
  padding: 0 var(--gl-space-6);
  background: rgba(255, 255, 255, 0.95);
  backdrop-filter: blur(12px);
  -webkit-backdrop-filter: blur(12px);
  border-bottom: 1px solid var(--gl-border-subtle);
}

.gl-navbar__logo {
  height: 28px;
  width: auto;
}

.gl-navbar__links {
  display: flex;
  align-items: center;
  gap: var(--gl-space-8);
  list-style: none;
  margin: 0;
  padding: 0;
}

.gl-navbar__link {
  font-family: var(--gl-font-body);
  font-weight: var(--gl-weight-medium);
  font-size: var(--gl-text-sm);
  color: var(--gl-text-secondary);
  text-decoration: none;
  transition: color var(--gl-transition-fast);
  position: relative;
}

.gl-navbar__link:hover,
.gl-navbar__link[aria-current="page"] {
  color: var(--gl-blue);
}

.gl-navbar__link[aria-current="page"]::after {
  content: '';
  position: absolute;
  bottom: -20px;
  left: 0;
  right: 0;
  height: 2px;
  background: var(--gl-blue);
  border-radius: 1px;
}

.gl-navbar__actions {
  display: flex;
  align-items: center;
  gap: var(--gl-space-3);
}

/* Dark variant (on blue or dark backgrounds) */
.gl-navbar--dark {
  background: rgba(15, 38, 71, 0.95);
  border-bottom-color: rgba(255, 255, 255, 0.08);
}

.gl-navbar--dark .gl-navbar__link {
  color: rgba(255, 255, 255, 0.72);
}

.gl-navbar--dark .gl-navbar__link:hover,
.gl-navbar--dark .gl-navbar__link[aria-current="page"] {
  color: var(--gl-white);
}

/* Mobile hamburger trigger (hidden on desktop) */
@media (max-width: 767px) {
  .gl-navbar__links {
    display: none;
  }

  .gl-navbar__mobile-toggle {
    display: flex;
  }
}

@media (min-width: 768px) {
  .gl-navbar__mobile-toggle {
    display: none;
  }
}
```

### Hero Section

```css
.gl-hero {
  position: relative;
  display: flex;
  align-items: center;
  min-height: 560px;
  padding: var(--gl-space-24) 0;
  overflow: hidden;
}

.gl-hero--gradient {
  background: var(--gl-gradient-standard);
  color: var(--gl-white);
}

.gl-hero--blue {
  background: var(--gl-blue);
  color: var(--gl-white);
}

.gl-hero--dark {
  background: var(--gl-shadow);
  color: var(--gl-white);
}

.gl-hero--light {
  background: var(--gl-bg-secondary);
  color: var(--gl-text-primary);
}

.gl-hero__content {
  position: relative;
  z-index: 1;
  max-width: 640px;
}

.gl-hero__label {
  display: inline-block;
  font-family: var(--gl-font-body);
  font-weight: var(--gl-weight-medium);
  font-size: var(--gl-text-xs);
  letter-spacing: 0.08em;
  text-transform: uppercase;
  margin-bottom: var(--gl-space-4);
  opacity: 0.72;
}

.gl-hero__title {
  font-family: var(--gl-font-heading);
  font-weight: var(--gl-weight-bold);
  font-size: var(--gl-text-6xl);                   /* 48px */
  line-height: var(--gl-leading-none);
  letter-spacing: -0.03em;
  margin-bottom: var(--gl-space-6);
}

@media (min-width: 1024px) {
  .gl-hero__title {
    font-size: var(--gl-text-7xl);                 /* 64px */
  }
}

.gl-hero__subtitle {
  font-family: var(--gl-font-body);
  font-size: var(--gl-text-lg);
  line-height: var(--gl-leading-normal);
  margin-bottom: var(--gl-space-8);
  opacity: 0.85;
}

.gl-hero__actions {
  display: flex;
  gap: var(--gl-space-4);
  flex-wrap: wrap;
}

@media (max-width: 767px) {
  .gl-hero {
    min-height: 400px;
    padding: var(--gl-space-16) 0;
  }

  .gl-hero__title {
    font-size: var(--gl-text-4xl);                 /* 36px */
  }

  .gl-hero__actions {
    flex-direction: column;
  }

  .gl-hero__actions .gl-btn {
    width: 100%;
  }
}
```

### Section Header

```css
.gl-section-header {
  text-align: center;
  max-width: 640px;
  margin: 0 auto var(--gl-space-16);
}

.gl-section-header__label {
  display: inline-block;
  font-family: var(--gl-font-body);
  font-weight: var(--gl-weight-medium);
  font-size: var(--gl-text-xs);
  letter-spacing: 0.08em;
  text-transform: uppercase;
  color: var(--gl-blue);
  margin-bottom: var(--gl-space-3);
}

.gl-section-header__title {
  font-family: var(--gl-font-heading);
  font-weight: var(--gl-weight-bold);
  font-size: var(--gl-text-4xl);                   /* 36px */
  line-height: var(--gl-leading-tight);
  letter-spacing: -0.02em;
  color: var(--gl-text-primary);
  margin-bottom: var(--gl-space-4);
}

.gl-section-header__description {
  font-family: var(--gl-font-body);
  font-size: var(--gl-text-lg);
  line-height: var(--gl-leading-normal);
  color: var(--gl-text-secondary);
}
```

### Footer

```css
.gl-footer {
  background: var(--gl-shadow);
  color: var(--gl-white);
  padding: var(--gl-space-16) 0 var(--gl-space-8);
}

.gl-footer__grid {
  display: grid;
  grid-template-columns: 2fr repeat(3, 1fr);
  gap: var(--gl-space-10);
  margin-bottom: var(--gl-space-12);
}

@media (max-width: 767px) {
  .gl-footer__grid {
    grid-template-columns: 1fr;
    gap: var(--gl-space-8);
  }
}

.gl-footer__brand {
  max-width: 280px;
}

.gl-footer__logo {
  height: 28px;
  margin-bottom: var(--gl-space-4);
}

.gl-footer__description {
  font-size: var(--gl-text-sm);
  line-height: var(--gl-leading-normal);
  color: rgba(255, 255, 255, 0.64);
}

.gl-footer__heading {
  font-family: var(--gl-font-heading);
  font-weight: var(--gl-weight-semibold);
  font-size: var(--gl-text-sm);
  color: var(--gl-white);
  margin-bottom: var(--gl-space-4);
}

.gl-footer__links {
  list-style: none;
  padding: 0;
  margin: 0;
  display: flex;
  flex-direction: column;
  gap: var(--gl-space-3);
}

.gl-footer__link {
  font-size: var(--gl-text-sm);
  color: rgba(255, 255, 255, 0.64);
  text-decoration: none;
  transition: color var(--gl-transition-fast);
}

.gl-footer__link:hover {
  color: var(--gl-white);
}

.gl-footer__bottom {
  padding-top: var(--gl-space-8);
  border-top: 1px solid rgba(255, 255, 255, 0.12);
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
  gap: var(--gl-space-4);
}

.gl-footer__copyright {
  font-size: var(--gl-text-xs);
  color: rgba(255, 255, 255, 0.48);
}
```

### Form Inputs

```css
.gl-input-group {
  display: flex;
  flex-direction: column;
  gap: var(--gl-space-2);
}

.gl-input-label {
  font-family: var(--gl-font-body);
  font-weight: var(--gl-weight-medium);
  font-size: var(--gl-text-sm);
  color: var(--gl-text-primary);
}

.gl-input {
  width: 100%;
  padding: var(--gl-space-3) var(--gl-space-4);    /* 12px 16px */
  font-family: var(--gl-font-body);
  font-size: var(--gl-text-base);
  line-height: var(--gl-leading-snug);
  color: var(--gl-text-primary);
  background: var(--gl-bg-primary);
  border: 1.5px solid var(--gl-border-default);
  border-radius: var(--gl-radius-md);
  transition: border-color var(--gl-transition-fast),
              box-shadow var(--gl-transition-fast);
}

.gl-input::placeholder {
  color: var(--gl-text-tertiary);
}

.gl-input:hover {
  border-color: var(--gl-gray-400);
}

.gl-input:focus {
  outline: none;
  border-color: var(--gl-blue);
  box-shadow: 0 0 0 3px var(--gl-blue-03);
}

.gl-input--error {
  border-color: var(--gl-error);
}

.gl-input--error:focus {
  box-shadow: 0 0 0 3px rgba(239, 68, 68, 0.15);
}

.gl-input-hint {
  font-size: var(--gl-text-xs);
  color: var(--gl-text-tertiary);
}

.gl-input-error {
  font-size: var(--gl-text-xs);
  color: var(--gl-error);
}

/* Textarea */
.gl-textarea {
  min-height: 120px;
  resize: vertical;
}

/* Select */
.gl-select {
  appearance: none;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='16' height='16' viewBox='0 0 24 24' fill='none' stroke='%2364748B' stroke-width='2' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpolyline points='6 9 12 15 18 9'%3E%3C/polyline%3E%3C/svg%3E");
  background-repeat: no-repeat;
  background-position: right 12px center;
  padding-right: var(--gl-space-10);
}
```

### Badges and Tags

```css
.gl-badge {
  display: inline-flex;
  align-items: center;
  gap: var(--gl-space-1);
  padding: 2px var(--gl-space-2);
  font-family: var(--gl-font-body);
  font-weight: var(--gl-weight-medium);
  font-size: var(--gl-text-xs);
  line-height: 1.5;
  border-radius: var(--gl-radius-full);
  white-space: nowrap;
}

.gl-badge--blue {
  background: var(--gl-blue-03);
  color: var(--gl-blue);
}

.gl-badge--green {
  background: var(--gl-green-03);
  color: #059669;
}

.gl-badge--horizon {
  background: var(--gl-horizon-03);
  color: #0891B2;
}

.gl-badge--shadow {
  background: var(--gl-shadow-03);
  color: var(--gl-shadow);
}

.gl-badge--error {
  background: var(--gl-error-bg);
  color: var(--gl-error);
}

.gl-badge--warning {
  background: var(--gl-warning-bg);
  color: #D97706;
}

/* Tag (clickable / removable variant) */
.gl-tag {
  display: inline-flex;
  align-items: center;
  gap: var(--gl-space-1);
  padding: var(--gl-space-1) var(--gl-space-3);
  font-family: var(--gl-font-body);
  font-weight: var(--gl-weight-medium);
  font-size: var(--gl-text-xs);
  border: 1px solid var(--gl-border-default);
  border-radius: var(--gl-radius-sm);
  background: var(--gl-bg-primary);
  color: var(--gl-text-secondary);
  cursor: pointer;
  transition: all var(--gl-transition-fast);
}

.gl-tag:hover {
  border-color: var(--gl-blue);
  color: var(--gl-blue);
  background: var(--gl-blue-03);
}

.gl-tag--active {
  border-color: var(--gl-blue);
  color: var(--gl-blue);
  background: var(--gl-blue-03);
}
```

---

## Gradient Patterns

### Standard 4-Color (Hero/Feature backgrounds)

```css
.gl-gradient-standard {
  background: var(--gl-gradient-standard);
  /* linear-gradient(135deg, #0058EA 0%, #00C0FE 35%, #01D3B8 65%, #0F2647 100%) */
}
```

### Duotone (Covers, footers)

```css
.gl-gradient-duotone {
  background: var(--gl-gradient-duotone);
  /* linear-gradient(135deg, #0058EA 0%, #0F2647 100%) */
}
```

### Freeform (Creative / editorial)

For freeform gradient blobs, use radial gradients positioned organically:

```css
.gl-gradient-freeform {
  background:
    radial-gradient(ellipse at 20% 30%, rgba(0, 88, 234, 0.6) 0%, transparent 60%),
    radial-gradient(ellipse at 80% 20%, rgba(0, 192, 254, 0.5) 0%, transparent 50%),
    radial-gradient(ellipse at 60% 80%, rgba(1, 211, 184, 0.4) 0%, transparent 50%),
    radial-gradient(ellipse at 30% 70%, rgba(15, 38, 71, 0.5) 0%, transparent 60%);
  background-color: #0F2647;
}
```

### Gradient Text

```css
.gl-gradient-text {
  background: var(--gl-gradient-blue);
  -webkit-background-clip: text;
  background-clip: text;
  -webkit-text-fill-color: transparent;
}
```

### Rules

- Gradients are **digital only** -- never reproduce in print.
- Always ensure text over gradient meets WCAG AA contrast.
- Use a semi-transparent dark overlay if needed: `rgba(15, 38, 71, 0.4)`.
- Gradient borders: use `border-image` or a pseudo-element approach.

---

## Animation and Transitions

### Standard Durations

| Token | Duration | Easing | Usage |
|---|---|---|---|
| `--gl-transition-fast` | 150ms | ease | Micro-interactions (hover color, opacity) |
| `--gl-transition-base` | 200ms | ease | Default hover states, focus rings |
| `--gl-transition-slow` | 300ms | ease | Expand/collapse, modal open |
| `--gl-transition-page` | 300ms | ease-in-out | Page-level transitions, route changes |

### Entrance Animations

```css
@keyframes gl-fade-in {
  from { opacity: 0; }
  to { opacity: 1; }
}

@keyframes gl-slide-up {
  from { opacity: 0; transform: translateY(16px); }
  to { opacity: 1; transform: translateY(0); }
}

@keyframes gl-scale-in {
  from { opacity: 0; transform: scale(0.95); }
  to { opacity: 1; transform: scale(1); }
}

.gl-animate-fade-in {
  animation: gl-fade-in 300ms ease forwards;
}

.gl-animate-slide-up {
  animation: gl-slide-up 400ms ease forwards;
}

.gl-animate-scale-in {
  animation: gl-scale-in 200ms ease forwards;
}
```

### Staggered Entrance

For lists of cards or items entering sequentially:

```css
.gl-stagger > * {
  opacity: 0;
  animation: gl-slide-up 400ms ease forwards;
}

.gl-stagger > *:nth-child(1) { animation-delay: 0ms; }
.gl-stagger > *:nth-child(2) { animation-delay: 80ms; }
.gl-stagger > *:nth-child(3) { animation-delay: 160ms; }
.gl-stagger > *:nth-child(4) { animation-delay: 240ms; }
.gl-stagger > *:nth-child(5) { animation-delay: 320ms; }
.gl-stagger > *:nth-child(6) { animation-delay: 400ms; }
```

### Rules

- **Respect prefers-reduced-motion:**
  ```css
  @media (prefers-reduced-motion: reduce) {
    *, *::before, *::after {
      animation-duration: 0.01ms !important;
      animation-iteration-count: 1 !important;
      transition-duration: 0.01ms !important;
    }
  }
  ```
- Never use bounce, elastic, or spring easings. Keep it professional.
- Hover transitions: 200ms maximum. Anything longer feels sluggish.
- Do not animate layout properties (width, height, top, left). Use transform and opacity only.

---

## Accessibility Requirements

### Contrast Ratios (WCAG AA)

| Text Type | Minimum Ratio | Verified Pairs |
|---|---|---|
| Normal text (< 18px) | 4.5:1 | Black on White (21:1), White on `#0058EA` (4.6:1), White on `#0F2647` (13.5:1) |
| Large text (>= 18px bold or >= 24px) | 3:1 | White on `#00C0FE` (3.1:1 -- large text only) |
| UI components / icons | 3:1 | `#0058EA` on White (4.6:1) |

### Critical Contrast Notes

- `#00C0FE` (Clear Horizon) fails AA for normal text on white. Use only for large text, icons, or decorative elements on light backgrounds.
- `#01D3B8` (Neo Green) fails AA for text on white. Use only as badge backgrounds, chart accents, or decorative. Never as text color on white.
- On gradient backgrounds, add a semi-transparent overlay to guarantee text contrast.

### Focus States

All interactive elements must have a visible focus indicator:

```css
*:focus-visible {
  outline: 2px solid var(--gl-blue);
  outline-offset: 2px;
}
```

### Keyboard Navigation

- All interactive elements must be reachable via Tab.
- Dropdown menus and modals must trap focus.
- Escape key must close modals and dropdowns.
- Skip-to-content link as the first focusable element.

### Semantic HTML Checklist

- Use `<nav>` for navigation, `<main>` for primary content, `<section>` with `aria-label` for distinct sections.
- Images must have `alt` text. Decorative images use `alt=""`.
- Form inputs must have associated `<label>` elements.
- Buttons use `<button>`, links use `<a>`. Never use `<div>` with click handlers.
- Use heading hierarchy (h1 -> h2 -> h3) without skipping levels.

---

## Concentric Effect (CSS)

For the brand-specific concentric ring decoration in web UI:

```css
.gl-concentric {
  position: relative;
}

.gl-concentric::before {
  content: '';
  position: absolute;
  width: 300px;
  height: 300px;
  border-radius: 50%;
  pointer-events: none;
  background: none;
  /* 4 concentric rings via box-shadow */
  box-shadow:
    0 0 0 40px rgba(255, 255, 255, 0.06),
    0 0 0 80px rgba(255, 255, 255, 0.08),
    0 0 0 120px rgba(255, 255, 255, 0.10),
    0 0 0 160px rgba(255, 255, 255, 0.04);
}

/* Position variants */
.gl-concentric--top-right::before {
  top: -120px;
  right: -120px;
}

.gl-concentric--bottom-left::before {
  bottom: -120px;
  left: -120px;
}

/* Light background variant */
.gl-concentric--light::before {
  box-shadow:
    0 0 0 40px rgba(0, 88, 234, 0.04),
    0 0 0 80px rgba(0, 88, 234, 0.06),
    0 0 0 120px rgba(0, 88, 234, 0.08),
    0 0 0 160px rgba(0, 88, 234, 0.03);
}
```

---

## Output Checklist

Before delivering any Gogolook web interface, verify:

- [ ] **CSS custom properties** use the `--gl-` prefix and match the token values above
- [ ] **Color proportions** approximate 50/20/20/10 (Blue / Shadow / Horizon / Green) across the page
- [ ] **Typography** uses Plus Jakarta Sans for headings, Inter for body text
- [ ] **Fonts are loaded** via Google Fonts with `display=swap`
- [ ] **Spacing** uses only values from the spacing scale (4-120px)
- [ ] **Border radius** uses tokens, not arbitrary values
- [ ] **Shadows** use the Shadow Blue-tinted tokens, not generic black
- [ ] **Buttons** have hover, active, focus-visible, and disabled states
- [ ] **Forms** have labels, focus states, error states, and hint text
- [ ] **Navigation** is sticky with backdrop blur, responsive hamburger on mobile
- [ ] **Grid** uses 12 columns with 24px gutters on desktop, stacking on mobile
- [ ] **Container** maxes out at 1200px and is centered
- [ ] **Dark mode** uses Shadow Blue backgrounds, not pure black
- [ ] **Gradients** are digital only, never in print; text contrast is verified
- [ ] **Animations** respect `prefers-reduced-motion`; only transform/opacity are animated
- [ ] **Contrast** meets WCAG AA (4.5:1 normal text, 3:1 large text and UI)
- [ ] **Focus indicators** are visible on all interactive elements (2px Blue outline)
- [ ] **Semantic HTML** is used (nav, main, section, button, label)
- [ ] **Concentric Effect** (if used) has max one per section, rings do not overlap text
