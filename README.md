# Confirm Design System — Component Library

> Extracted from the [Confirm Design System Figma file](https://www.figma.com/design/j6GnhZh97kbTqMydn18ns8/Confirm-Design-System) · By Siemens BSW

## 🔗 Live Links

| Page | URL |
|---|---|
| 📖 **Token Reference** | [View →](https://poorva007.github.io/Confirm-Design-Components/tokens-reference.html) |
| 🖥️ **Work Orders Dashboard** | [View →](https://poorva007.github.io/Confirm-Design-Components/) |

---

## 📦 What's in this repo

| File | Description |
|---|---|
| [`tokens.css`](tokens.css) | All CSS custom properties — drop into your `:root {}` |
| [`tokens-reference.html`](tokens-reference.html) | Interactive token reference for developers |
| [`index.html`](index.html) | Full Work Orders dashboard prototype |

---

## 🎨 Design Tokens

All tokens extracted directly from the Figma variable collections via the Figma REST API.

### Colors (31 tokens)
- **Base palette** — `--color-base-0` → `--color-base-4`
- **Brand** — `--color-brand-primary` (`#017d80`), `--color-brand-dark` (`#002743`), `--color-brand-accent` (`#48fe9b`)
- **Text** — default, inverse, secondary, active, soft, weak, alt, alarm
- **Borders** — default, soft, weak, focus, alarm, success, info, warning
- **Status backgrounds** — success, failure, info, warning

### Typography (34 styles)
- **Font:** Yellix TRIAL (fallback: Inter, system-ui)
- **Weights:** 350 (regular) · 700 (bold)
- **Scale:** Display 01–03 · H1–H5 · Body LG/MD/SM · Label LG/MD/SM/XS

### Spacing (7 steps)
`2px` · `4px` · `8px` · `12px` · `16px` · `24px` · `32px`

### Border Radius
`--radius-4` · `--radius-8` · `--radius-full (100px)`

### Shadows
`--shadow-sm` · `--shadow-md` · `--shadow-lg`

---

## 🚀 Quick Start

```html
<!-- 1. Add tokens to your project -->
<link rel="stylesheet" href="tokens.css" />

<!-- 2. Use tokens in your CSS -->
<style>
  .btn-primary {
    background: var(--color-primary-default);   /* #017d80 */
    color:      var(--color-text-inverse);       /* #ffffff */
    border-radius: var(--radius-4);             /* 4px     */
    font-size:  var(--type-label-lg-size);       /* 14px    */
    padding:    0 var(--spacing-12);            /* 0 12px  */
  }
</style>
```

---

## 🔄 Re-extracting tokens

Tokens were extracted using the Figma REST API:

```bash
# Styles
curl -H "X-Figma-Token: YOUR_TOKEN" \
  "https://api.figma.com/v1/files/j6GnhZh97kbTqMydn18ns8/styles"

# Variables (design tokens)
curl -H "X-Figma-Token: YOUR_TOKEN" \
  "https://api.figma.com/v1/files/j6GnhZh97kbTqMydn18ns8/variables/local"
```

---

*Last extracted: June 2026 · Figma file: `j6GnhZh97kbTqMydn18ns8`*
