# delightful-ghostty

Ghostty terminal theme using the Delightful OKLCH palette. Light and dark theme files are the portable artifact; `config` and `shaders/` are optional, opinionated extras.

## Source of Truth

Token hex values come from [delightful.build](https://delightful.build/) and the `delightful-design-system` repo. This repo intentionally keeps its own hex snapshots because Ghostty themes require hex values.

## Validate

- Inspect `themes/delightful-light` and `themes/delightful-dark` for valid Ghostty `key = value` syntax.
- Confirm all hex values are six-digit lowercase hex strings.
- Confirm terminal palette slots match `delightful-iterm2` where both ports expose the same ANSI slot.
- Check README raw GitHub URLs after changing filenames.

## Editing Rules

- Edit theme files directly only when the canonical palette changes.
- Keep blue terminal slots mapped to Delightful cyan; there is no dedicated blue family.
- Treat `config` as personal/opinionated. Theme files are the public install surface.
- Keep shader filenames in docs synchronized with `shaders/*.glsl`.

## Screenshots

Screenshots in `screenshots/` should show real Ghostty light and dark sessions using these theme files. Refresh them only when theme colors, font settings, or config-visible chrome changes.
