# Kiddie Genius World 🌍

A child-friendly educational web app designed to make learning fun, safe, and accessible for kids aged 2–10.

---

## Screenshots

| Above the fold |
|---|
| ![Above the fold](https://github.com/user-attachments/assets/88d98aca-cbac-4e0d-8303-e0f6f34c08b5) |

---

## Mascot — Gray the Cheetah Cub 🐆

**Gray** is a 4-year-old cartoon cheetah cub and the mascot/narrator of Kiddie Genius World. He wears a blue baseball cap bearing the Kiddie Genius World globe logo and has bright blue eyes.

| Location | Role |
|----------|------|
| **Hero** | Greets kids with a speech bubble: *"Hi! I'm Gray! Let's learn something amazing today!"* |
| **Activities** | Narrator tip box above the activity cards |
| **Meet Gray** | Dedicated section introducing Gray to new users |
| **Footer** | Waves goodbye at the bottom of the page |

To use the official character art, overwrite `assets/gray.svg` with the real photo (`Graycheetah3.jpg`) and update the `src` in `index.html`.

---

## Brand Assets

| File | Usage |
|------|-------|
| `assets/logo.svg` | Globe logo in header, about section, footer |
| `assets/gray.svg` | Gray the cheetah mascot throughout |

### Cover Banner

The hero banner uses the **official Facebook cover photo** (`fbcoverkgw.png`) loaded from GitHub CDN.
If that URL is unavailable (local dev without internet), an `onerror` handler activates a CSS fallback
banner (`.brand-banner--css`) that replicates the sky-blue gradient and rainbow brand text.

**For production:** either keep the GitHub CDN URL or download `fbcoverkgw.png` to `assets/cover.png`
and update the `src` attribute.

---

## Design System

### Typography

| Token | Value | Usage |
|-------|-------|-------|
| `--font-primary` | `'Nunito'` (Google Fonts) | All UI text |
| `--fs-xs` – `--fs-3xl` | 14 px – 48 px scale | Headings, body, labels |

**Why Nunito?** Fully rounded terminals match the official logo lettering style. Weights 400–900 only.

### Colour Palette — extracted from the cover artwork lettering

| Token | Hex | Source |
|-------|-----|--------|
| `--clr-red` | `#e63329` | "Kiddie" red |
| `--clr-yellow` | `#ffc107` | "Genius" yellow |
| `--clr-green` | `#4caf28` | "World" green |
| `--clr-blue` | `#2b7de9` | Globe ocean / sky |
| `--clr-navy` | `#162b6e` | Logo outline |
| `--clr-orange` | `#fd7c1e` | Rocket / warmth |

All pairings meet **WCAG AA** contrast (4.5:1 normal, 3:1 large text).

### Spacing & Tap Targets

- Minimum button height: **52 px** (large enough for small hands)
- Card padding: `2rem`; grid gap: `2rem`
- Border-radius: `0.75rem` → `9999px` (pills) for a soft, friendly feel

---

## Getting Started

No build step required — pure HTML + CSS.

```bash
open index.html
# or
python3 -m http.server 8080
```

Deploy to **Netlify**: upload `KiddieGenius_Build.zip` via the dashboard.

---

## Accessibility

- `:focus-visible` outlines on all interactive elements (yellow, 3 px)
- `aria-label` / `role` on cards and icon-only controls
- Semantic HTML5 landmarks throughout
- Responsive: 320 px → 1400 px

---

## License

MIT © 2025 Daniel Cook
