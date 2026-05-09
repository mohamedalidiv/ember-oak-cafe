# Ember & Oak — Specialty Café
### Where Every Bean Tells a Story

---

## Overview

**Ember & Oak** is a single-page, fully responsive café website built with pure HTML and CSS — no frameworks, no dependencies. The design blends **minimalist editorial structure** with **warm tactile aesthetics**, targeting a discerning audience that values design as much as quality coffee.

The visual identity sits at the intersection of rustic warmth and high-end sophistication — evoking the sensory experience of a specialty café: the aroma of roasted beans, the texture of reclaimed oak, and the quiet comfort of a morning ritual.

---

## Tech Stack

- **HTML5** — semantic, single-file architecture
- **CSS3** — custom properties (design tokens), CSS Grid, Flexbox, CSS masonry
- **Google Fonts** — Playfair Display (headlines) + Inter (body/UI)
- **Unsplash** — photography via CDN
- **No JavaScript** — fully static, zero dependencies

---

## Sections

| Section | Description |
|---------|-------------|
| **Header / Nav** | Sticky glassmorphism navbar with active dot indicator |
| **Hero** | Full-viewport hero with subtle background image overlay |
| **About** | Two-column grid: content + image with gradient overlay |
| **Menu** | Tab navigation + 4-column card grid with hover zoom |
| **Features** | 3-column feature card grid with emoji icons |
| **Gallery** | CSS masonry layout (columns-based) with hover scale |
| **Testimonials** | 3-column review cards with star ratings |
| **Reservation** | 2-column form with terracotta focus states |
| **Footer** | Brand column + navigation links + copyright bar |

---

## Design System — Full Spec in [`DESIGN.md`](./DESIGN.md)

### Color Palette
| Token | Hex | Role |
|-------|-----|------|
| `primary` | `#0d0300` | Deep Espresso — main typography & dark elements |
| `secondary` | `#934a27` | Muted Terracotta — CTAs, accents, active states |
| `secondary-container` | `#ffa277` | Soft Amber — chips, avatar backgrounds |
| `surface` | `#fff9ef` | Warm Cream — page canvas |
| `on-surface` | `#1f1b0f` | Warm Black — body text |
| `surface-container` | `#f6edd8` | Elevated surfaces — cards, footer |
| `tertiary-fixed-dim` | `#fdba49` | Star rating gold |

### Typography
| Style | Font | Size | Usage |
|-------|------|------|-------|
| `headline-xl` | Playfair Display 700 | 48px | Hero title |
| `headline-lg` | Playfair Display 600 | 32px | Section titles |
| `headline-md` | Playfair Display 600 | 24px | Card titles |
| `body-lg` | Inter 400 | 18px | Hero description |
| `body-md` | Inter 400 | 16px | General body text |
| `label` | Inter 600 | 14px | Tags, nav, badges (uppercase + tracked) |

### Shape Language
- **Buttons & Inputs:** `14px` radius — "Softened Geometry"
- **Cards & Containers:** `18px` radius
- **Reservation box:** `24px` radius
- **Chips / Tags:** `999px` (pill) — for flavor badges only
- **No fully circular buttons** — maintains architectural brand feel

### Elevation Rules
- Shadows use warm espresso tint: `rgba(44, 26, 14, 0.08)` — never cold black
- Hover lift: `translateY(-6px)` on cards, `translateY(-2px)` on buttons
- Image gradient overlay: `rgba(0,0,0,.35)` from bottom
- Nav backdrop: `backdrop-filter: blur(12px)` + 90% surface opacity

---

## Key CSS Patterns

```css
/* Design tokens via CSS custom properties */
:root {
  --surface: #fff9ef;
  --primary: #0d0300;
  --secondary: #934a27;
  --shadow: rgba(44, 26, 14, .08);
  --section-gap: 80px;
  --radius: 16px;
}

/* Masonry gallery — pure CSS, no JS */
.gallery {
  columns: 3 300px;
  column-gap: 24px;
}

/* Active nav dot indicator — no underline */
nav a.active::after {
  content: '';
  position: absolute;
  bottom: -10px;
  width: 6px;
  height: 6px;
  border-radius: 50%;
  background: var(--secondary);
}
```

---

## Responsive Breakpoints

| Breakpoint | Changes |
|------------|---------|
| `≤ 1100px` | Menu, features, testimonials → 2-column |
| `≤ 900px` | Nav hidden, about → single column, form → single column |
| `≤ 700px` | Container padding reduced, headlines shrink, all grids → 1-column |

---

## File Structure

```
ember-oak/
├── index.html      # All HTML, CSS, and content in one file
└── DESIGN.md       # Full design system specification
```

---

## Setup

No build step required. Open directly in a browser:

```bash
# Option 1 — just open the file
open index.html

# Option 2 — local server
npx serve .
# or
python3 -m http.server 8080
```

---

## Brand Voice

> *"Where the warmth of reclaimed oak meets the precision of modern brewing."*

Ember & Oak positions itself as a **sanctuary** — a neighborhood anchor for designers, writers, and coffee purists. Every design decision reinforces this: aggressive whitespace, editorial type pairing, warm tonal shadows, and product chips that label experiences ("Smooth," "Bold," "Fruity") rather than just ingredients.

---

*© 2024 Ember & Oak Specialty Café. Est. 2018.*
