
# NEXUS-7 | Cyborg Theme Landing Page

A fully responsive, single-file HTML landing page built around a dark sci-fi cyborg aesthetic. No frameworks or build tools required — open in any modern browser.

---

## Files

| File | Description |
|------|-------------|
| `cyborg-landing.html` | Complete landing page (HTML + CSS + JS in one file) |
| `README.md` | This document |

---

## Sections

| Section | ID | Description |
|---------|----|-------------|
| Navigation | — | Fixed top bar with logo, nav links, and CTA button |
| Hero | — | Full-viewport intro with animated cyborg SVG figure |
| Features | `#features` | 6-card augmentation module grid |
| Augmentation Metrics | `#aug` | Split layout with list + animated progress bars |
| Testimonials | `#trials` | 3-column trial subject quote cards |
| CTA / Enroll | `#enroll` | Email capture form with background text effect |
| Footer | — | Logo, copyright, and utility links |

---

## Design System

### Color Palette

| Variable | Hex | Usage |
|----------|-----|-------|
| `--cyan` | `#00f5ff` | Primary accent, glows, highlights |
| `--red` | `#ff2a2a` | Secondary accent, section tags |
| `--dark` | `#020408` | Page background |
| `--panel` | `#040d14` | Card / section backgrounds |
| `--text` | `#c8e8f0` | Body text |
| `--dim` | `#4a7a8a` | Muted / secondary text |

### Typography

| Font | Weight | Usage |
|------|--------|-------|
| `Orbitron` | 400 / 700 / 900 | Headings, logo, stat numbers |
| `Rajdhani` | 300 / 400 / 600 | Body text, descriptions |
| `Share Tech Mono` | 400 | Labels, tags, monospaced UI elements |

All fonts are loaded from Google Fonts via CDN.

---

## Features & Effects

- **Custom cursor** — smooth-tracking ring cursor with red highlight on hover over interactive elements
- **Scanline overlay** — full-page CRT scanline texture via CSS `repeating-linear-gradient`
- **Animated grid background** — perspective-scrolling grid in the hero section
- **Floating cyborg SVG** — hand-crafted SVG illustration with floating animation, scan line, and HUD data points
- **Rotating rings** — CSS `spin` keyframe rings around the cyborg figure
- **Glitch effect** — flicker animation on the hero headline
- **Counter animation** — stats count up on scroll into view (IntersectionObserver)
- **Progress bars** — animated fill bars that re-trigger on scroll
- **Clip-path buttons** — angled parallelogram-style button shapes
- **Corner bracket UI** — decorative corner accents on the hero visual panel
- **Smooth scroll** — native `scroll-behavior: smooth` + JS fallback for anchor links

---

## Responsive Breakpoints

| Breakpoint | Layout Changes |
|------------|---------------|
| > 900px | Full two-column hero, 3-column features, cyborg visual visible |
| ≤ 900px | Single-column hero, hidden cyborg visual, stacked features and nav |

---

## Browser Support

Works in all modern browsers (Chrome, Firefox, Safari, Edge). Requires:
- CSS custom properties
- CSS `clip-path`
- `IntersectionObserver` API
- Google Fonts CDN access

---

## How to Use

1. Download `cyborg-landing.html`
2. Open directly in a browser — no server required
3. Customize the CSS variables in `:root` to retheme instantly
4. Replace placeholder text / form action with real content

### Quick Theme Swap

```css
:root {
  --cyan: #00f5ff;   /* change to any accent color */
  --red:  #ff2a2a;   /* change secondary accent */
  --dark: #020408;   /* change page background */
}
```

---

## Customization Guide

| What to change | Where |
|----------------|-------|
| Brand name | `.nav-logo`, `.footer-logo`, `<title>` |
| Hero headline | `.hero-title` spans |
| Stats numbers | `animCounter()` calls in `<script>` |
| Feature cards | `.feat-card` blocks in `#features` |
| Progress bar values | `width` inline style + `.progress-val` text |
| Testimonials | `.testi-card` blocks in `#trials` |
| CTA form action | Add `action=""` to `.cta-form` or wire up JS |

---

## License

Free to use for personal and commercial projects. Attribution appreciated but not required.
