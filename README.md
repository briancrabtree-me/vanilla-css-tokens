# vanilla-css-tokens

Acid-on-dark CSS custom properties and optional layout primitives. No build step, no utilities framework. Use in **any** HTML page, static site, or framework — not tied to a specific starter.

[![License: MIT](https://img.shields.io/badge/License-MIT-ccff00?style=flat-square)](LICENSE)
[![Example](https://img.shields.io/badge/example-layout.html-ccff00?style=flat-square)](https://github.com/briancrabtree-me/vanilla-css-tokens/blob/main/examples/layout.html)

**[Example](examples/layout.html)** · **[snippet-library](https://github.com/briancrabtree-me/snippet-library)** · **[react-pubsub-store](https://github.com/briancrabtree-me/react-pubsub-store)** · **[pure-react-19-vanilla-starter](https://github.com/briancrabtree-me/pure-react-19-vanilla-starter)** · **[briancrabtree.me](https://briancrabtree.me/)**

**Viewing the example:** Open [`examples/layout.html`](examples/layout.html) in a browser (uses jsDelivr). GitHub’s file preview may not load relative CSS — you would see a blank page without the CDN links in that file.

---

## Install

Load tokens first, then UI (optional):

```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/briancrabtree-me/vanilla-css-tokens@main/tokens.css" />
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/briancrabtree-me/vanilla-css-tokens@main/ui.css" />
```

```css
@import './tokens.css';
@import './ui.css';
```

## Files

| File | Role |
|------|------|
| `tokens.css` | `:root` custom properties |
| `ui.css` | Header, nav, main, hero, cards, buttons, footer |
| `examples/layout.html` | Static demo (open locally or on GitHub) |

## Usage

RGB channels — add alpha in one place:

```css
body {
  background: rgb(var(--bg-main));
  color: rgb(var(--text-main));
}

.card {
  background: rgb(var(--bg-surface));
  border: 1px solid rgb(var(--border));
}
```

Override any token on `:root` in your own stylesheet to customize the palette.

## Tokens

| Token | Role |
|-------|------|
| `--bg-main` | Page background |
| `--bg-surface` | Cards, nav, panels |
| `--text-main` | Body text |
| `--text-dim` | Secondary text |
| `--accent` | Acid highlight (`#ccff00`) |
| `--on-accent` | Text on accent surfaces |
| `--border` | Hairline borders |
| `--gap-xs` … `--gap-2xl` | Spacing scale |
| `--container-pad`, `--section-pad-y`, `--footer-pad` | Page rhythm |
| `--nav-h` | Sticky header height |
| `--max-w` | Content max width |
| `--font-sans`, `--text-sm` … `--text-hero` | Type scale |
| `--z-header` | Header stacking |
| `--radius-none`, `--radius-sm` | Corners |
| `--color-focus`, `--color-error` | Focus and errors |

## UI classes

| Class | Role |
|-------|------|
| `.ui-header`, `.ui-nav`, `.ui-brand`, `.ui-nav-links` | Sticky header and menu |
| `.ui-main` | Centered content column |
| `.ui-hero`, `.ui-hero-title`, `.ui-hero-lead`, `.ui-hero-cta` | Text hero |
| `.ui-section-title`, `.ui-grid`, `.ui-card` | Section and card grid |
| `.ui-btn`, `.ui-btn-primary` | Buttons and CTA links |
| `.ui-footer` | Page footer |

## License

MIT — [LICENSE](LICENSE).
