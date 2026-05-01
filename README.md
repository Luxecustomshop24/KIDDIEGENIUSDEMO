# KiddieGenius 🧠

A child-friendly educational web app designed to make learning fun, safe, and accessible for kids aged 2–10.

---

## Design System

### Typography

| Token | Value | Usage |
|-------|-------|-------|
| `--font-primary` | `'Nunito'` (Google Fonts) | All UI text |
| `--fs-xs` – `--fs-3xl` | 14 px – 48 px scale | Headings, body, labels |

**Why Nunito?**  
Nunito uses fully rounded terminals making letters easy to distinguish. It is optimised for screen readability at small sizes and has a friendly, approachable personality — ideal for children. Only weights 400, 600, 700, 800, and 900 are loaded to keep page load fast.

---

### Colour Palette

| Token | Hex | Use |
|-------|-----|-----|
| `--clr-bg` | `#fffbf0` | Page background (warm cream) |
| `--clr-primary` | `#ff6b6b` | CTA buttons, logo |
| `--clr-secondary` | `#4ecdc4` | Secondary actions |
| `--clr-accent` | `#ffe66d` | Badges, highlights |
| Card purples/oranges/greens/blues/pinks/yellows | — | Activity card accents |

All foreground-background colour pairings meet **WCAG AA** minimum contrast (4.5 : 1 for normal text, 3 : 1 for large text).

---

### Spacing & Sizing

- Minimum tap target: **52 px** (buttons) for small-hand accessibility.
- Cards use generous `padding: 1.5 rem` and `gap: 2 rem` grid spacing.
- `border-radius` tokens range from `0.75 rem` (small) to `9999 px` (pill buttons) for a consistently soft, friendly look.

---

### Component Highlights

| Component | Child-Friendly Features |
|-----------|------------------------|
| **Header** | Sticky, large logo, pill nav links that highlight on hover |
| **Hero** | Animated floating emoji bubbles, large CTA button |
| **Activity Cards** | Colour-coded top borders, emoji icons, hover lift effect, `tabindex` for keyboard access |
| **Badges** | Translucent glass cards on a purple gradient; scale on hover |
| **Footer** | Dark background, readable contrast, simple links |

---

## Getting Started

The app is a **static HTML + CSS** site with no build step required.

```bash
# Open locally
open index.html
```

For deployment to Netlify (or any static host), zip `index.html`, `styles.css`, and `_redirects` and upload — or use the pre-built `KiddieGenius_Build.zip`.

---

## Accessibility

- All interactive elements have visible `:focus-visible` outlines.
- `aria-label` attributes are provided on icon-only controls.
- `role="button"` and `tabindex="0"` on card elements allow keyboard navigation.
- Semantic HTML5 landmark elements (`<header>`, `<main>`, `<footer>`, `<nav>`, `<section>`, `<article>`).

---

## License

MIT © 2025 Daniel Cook
