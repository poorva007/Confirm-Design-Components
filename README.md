# Confirm Design System — Component Library

> Extracted from the [Confirm Design System Figma file](https://www.figma.com/design/j6GnhZh97kbTqMydn18ns8/Confirm-Design-System) · By Siemens BSW

## 🔗 Live Links

| Page | URL |
|---|---|
| 📖 **Token Reference** | [poorva007.github.io/…/tokens-reference.html](https://poorva007.github.io/Confirm-Design-Components/tokens-reference.html) |
| 🧩 **Component Library** | [poorva007.github.io/…/components/](https://poorva007.github.io/Confirm-Design-Components/components/) |
| 🖥️ **Work Orders Dashboard** | [poorva007.github.io/…/](https://poorva007.github.io/Confirm-Design-Components/) |

---

## 📦 Repository Structure

```
├── tokens.css                  ← All CSS custom properties (66 tokens)
├── tokens-reference.html       ← Interactive token docs for developers
├── index.html                  ← Work Orders dashboard prototype
└── components/
    ├── index.html              ← Component gallery
    ├── button.html             ← Button (primary/secondary/ghost/danger)
    ├── accordion.html          ← Accordion (closed/open/flush)
    ├── checkbox-toggle.html    ← Checkbox, Toggle, Radio buttons
    ├── dropdown.html           ← Dropdown (default/search/selected)
    ├── pagination.html         ← Pagination (full/minimal/toolbar)
    ├── filter.html             ← Filter bar + advanced filter panel
    └── table.html              ← Table with accordion rows & pagination
```

---

## 🎨 Design Tokens (extracted via Figma REST API)

### Colors (31)
| Group | Tokens |
|---|---|
| Base palette | `--color-base-0` → `--color-base-4` |
| Brand | `--color-brand-primary` (#017d80), `--color-brand-dark` (#002743), `--color-brand-accent` (#48fe9b) |
| Text | default · inverse · secondary · active · soft · weak · alt · alarm |
| Borders | default · soft · weak · focus · alarm · success · info · warning |
| Status bg | success · failure · info · warning |
| Interactive | primary-default/hover/active/disabled · secondary-hover/active |

### Typography (34 styles)
- **Font:** Yellix TRIAL (fallback: Inter, system-ui)
- **Weights:** 350 (regular) · 700 (bold)
- **Scale:** Display 01–03 · H1–H5 · Body LG/MD/SM · Label LG/MD/SM/XS

### Spacing · Radius · Shadows
`2–32px` spacing · `4/8/100px` radii · `sm/md/lg` shadows

---

## 🚀 Quick Start

```html
<link rel="stylesheet" href="tokens.css" />

<style>
  .btn-primary {
    background:    var(--color-primary-default);  /* #017d80 */
    color:         var(--color-text-inverse);      /* #ffffff */
    border-radius: var(--radius-4);               /* 4px     */
    font-size:     var(--type-label-lg-size);      /* 14px    */
    padding:       0 var(--spacing-12);           /* 0 12px  */
  }
</style>
```

---

*Last extracted: June 2026 · Figma: `j6GnhZh97kbTqMydn18ns8`*
