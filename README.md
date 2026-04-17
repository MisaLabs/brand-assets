# MisaLabs Brand Assets

Official MisaLabs brand assets and design system reference for use in development, design, and AI-assisted workflows.

> **AI / Vibe-coding tip:** Drop any raw URL from this file directly into your prompt (Cursor, Claude, Copilot, etc.) and the assistant will pull the asset in automatically — no downloading needed.

---

## Quick Asset URLs

| Asset | Raw URL |
|-------|---------|
| Logo — wordmark (light) | `https://raw.githubusercontent.com/MisaLabs/brand-assets/main/logos/light/misalabs-wordmark.svg` |
| Logo — wordmark + symbol (light) | `https://raw.githubusercontent.com/MisaLabs/brand-assets/main/logos/light/misalabs-wordmark-symbol.svg` |
| Logo — symbol only (light) | `https://raw.githubusercontent.com/MisaLabs/brand-assets/main/logos/light/misalabs-symbol.svg` |
| Logo — wordmark (dark) | `https://raw.githubusercontent.com/MisaLabs/brand-assets/main/logos/dark/misalabs-wordmark.svg` |
| Logo — wordmark + symbol (dark) | `https://raw.githubusercontent.com/MisaLabs/brand-assets/main/logos/dark/misalabs-wordmark-symbol.svg` |
| Logo — symbol only (dark) | `https://raw.githubusercontent.com/MisaLabs/brand-assets/main/logos/dark/misalabs-symbol.svg` |

---

## Folder Structure

```
brand-assets/
├── logos/
│   ├── light/     # White/light logo — for dark backgrounds (UI, dark slides)
│   └── dark/      # Dark logo — for light/white backgrounds (docs, one-pagers)
└── icons/         # Favicon, app icon, standalone mark
```

---

## Design System

MisaLabs has two contexts with slightly different styling:

| Context | Font | Background | Usage |
|---------|------|------------|-------|
| **Product / UI** | Inter | Dark (`#0C0E12`) | Web app, dashboards, portals |
| **Sales / Slides** | Albert Sans | White or gradient | Decks, one-pagers, marketing |

---

## UI Design System (Product / Dark Mode)

The MisaLabs portal and product UI is dark-first, built with Inter and a tight set of design tokens.

### Colors

#### Backgrounds
| Token | Hex | Usage |
|-------|-----|-------|
| `bg-primary` | `#0C0E12` | Main app background |
| `bg-primary_alt` | `#13161B` | Alternate sections, sidebar |
| `bg-tertiary` | `#22262F` | Hover states, subtle fills |
| `bg-active` | `#22262F` | Active/selected items |
| `bg-brand-solid` | `#0D88A6` | Brand-colored button fills |

#### Text
| Token | Hex | Usage |
|-------|-----|-------|
| `text-primary` | `#F7F7F7` | Main body text, headings |
| `text-secondary` | `#CECFD2` | Supporting text |
| `text-tertiary` | `#94979C` | Captions, metadata |
| `text-placeholder` | `#85888E` | Input placeholders |
| `text-white` | `#FFFFFF` | Text on brand/colored surfaces |

#### Borders
| Token | Hex | Usage |
|-------|-----|-------|
| `border-primary` | `#373A41` | Default borders |
| `border-secondary` | `#22262F` | Subtle dividers |

#### Brand / Accent
| Token | Hex | Usage |
|-------|-----|-------|
| `utility-brand-300` | `#0B6F87` | Dark brand tint |
| `utility-brand-400` | `#0D88A6` | Brand mid / button fill |
| `utility-brand-500` | `#0F9CBE` | Primary brand accent |
| `utility-brand-600` | `#49BDDE` | Light brand highlight |
| `button-primary-icon` | `#73CDE6` | Icon inside brand buttons |

### Typography

| Role | Font | Weight | Size | Line Height |
|------|------|--------|------|-------------|
| Body (md) | Inter | 400 | 16px | 24px |
| Body (sm) | Inter | 400 | 14px | 20px |
| Body (xs) | Inter | 400 | 12px | 18px |
| Label (sm) | Inter | 500 | 14px | 20px |
| Label (md) | Inter | 500 | 16px | 24px |
| Semibold (sm) | Inter | 600 | 14px | 20px |
| Semibold (md) | Inter | 600 | 16px | 24px |
| Display (xs) | Inter | 600 | 24px | 32px |
| Display (sm) | Inter | 600 | 30px | 38px |
| Display (lg) | Inter | 600 | 48px | 60px / -2 letter-spacing |

```html
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap" rel="stylesheet">
```

```css
font-family: 'Inter', sans-serif;
```

### Spacing

| Token | Value |
|-------|-------|
| `spacing-xxs` | 2px |
| `spacing-xs` | 4px |
| `spacing-sm` | 6px |
| `spacing-md` | 8px |
| `spacing-lg` | 12px |
| `spacing-xl` | 16px |
| `spacing-2xl` | 20px |
| `spacing-3xl` | 24px |
| `spacing-4xl` | 32px |
| `spacing-5xl` | 40px |
| `spacing-6xl` | 48px |
| `spacing-7xl` | 64px |
| `container-padding-desktop` | 32px |
| `container-max-width-desktop` | 1280px |

### Border Radius

| Token | Value |
|-------|-------|
| `radius-xs` | 4px |
| `radius-sm` | 6px |
| `radius-md` | 8px |
| `radius-lg` | 10px |
| `radius-xl` | 12px |
| `radius-2xl` | 16px |
| `radius-full` | 9999px |

---

## Sales & Marketing Design System (Slides / One-pagers)

### Colors

| Name | Hex | Usage |
|------|-----|-------|
| Deep Navy | `#1F5477` | Headings, primary dark |
| Ocean Blue | `#0F9CBE` | Accent, CTAs, highlight cards |
| Sky Blue | `#81CCE3` | Secondary accent, captions |
| White | `#FFFFFF` | Slide backgrounds, text on dark |

### Gradient

```css
/* Standard brand gradient */
background: linear-gradient(to right, #1F5477, #0F9CBE);

/* Soft three-stop version */
background: linear-gradient(to right, #1F5477, #0F9CBE, #81CCE3);
```

### Typography

```html
<link href="https://fonts.googleapis.com/css2?family=Albert+Sans:wght@400;500;600;700&display=swap" rel="stylesheet">
```

```css
font-family: 'Albert Sans', sans-serif;
```

### Slide Style Rules

- **Background:** White `#FFFFFF` or brand gradient
- **Headings:** `#1F5477` on white; white on gradient/dark backgrounds
- **Accent / CTA text:** `#0F9CBE`
- **Captions / supporting text:** `#81CCE3`
- **Highlight cards:** `#0F9CBE` fill with white bold text
- **Comparison winner column:** Ocean Blue fill, white text

---

## AI Prompt Snippets

### For UI / Product work
```
Use the MisaLabs UI design system (dark mode):
- Font: Inter (Google Fonts), weights 400/500/600
- Background: #0C0E12 (primary), #13161B (alt), #22262F (tertiary/hover)
- Text: #F7F7F7 (primary), #CECFD2 (secondary), #94979C (tertiary)
- Brand accent: #0F9CBE (primary), #49BDDE (light), #0D88A6 (dark)
- Borders: #373A41 (primary), #22262F (subtle)
- Border radius: 8px default, 6px small, 12px large
- Spacing base unit: 8px
- Logo: https://raw.githubusercontent.com/MisaLabs/brand-assets/main/logos/light/misalabs-wordmark-symbol.svg
```

### For Sales / Marketing / Slides
```
Use the MisaLabs brand style for sales materials:
- Font: Albert Sans (Google Fonts)
- Colors: Deep Navy #1F5477, Ocean Blue #0F9CBE, Sky Blue #81CCE3, White #FFFFFF
- Gradient: linear-gradient(to right, #1F5477, #0F9CBE)
- Style: Clean white background, teal/blue accents, bold navy headings
- Logo (dark, for white backgrounds): https://raw.githubusercontent.com/MisaLabs/brand-assets/main/logos/dark/misalabs-wordmark-symbol.svg
```

---

## Asset Naming Convention

```
misalabs-[type]-[variant].[ext]

Examples:
misalabs-wordmark.svg
misalabs-wordmark-symbol.svg
misalabs-symbol.svg
misalabs-symbol-256px.png
```

---

*For questions or to contribute assets, open a PR or contact the design team.*
