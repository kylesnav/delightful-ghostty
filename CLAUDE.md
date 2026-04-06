# delightful-ghostty

Ghostty terminal theme using the Delightful OKLCH palette. Light and dark variants.

## Source of Truth

Token hex values come from [delightful-design-system](https://github.com/kylesnav/delightful-design-system). This repo maintains its own hex copies in the theme files — no build step, no imports.

## Key Files

- `themes/delightful-light`, `themes/delightful-dark` — Ghostty theme files (palette hex values)
- `config` — Opinionated Ghostty settings (fonts, keybinds, window chrome). Separate from the theme.
- `shaders/` — Optional GLSL post-processing effects

## Conventions

- All colors are hex. The canonical source is OKLCH but Ghostty needs hex.
- Blue slots use the cyan hue (Delightful has no dedicated blue).
- Config is personal/opinionated — theme files are the portable part.
