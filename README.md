<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="screenshots/Ghostty-Dark.png" />
    <source media="(prefers-color-scheme: light)" srcset="screenshots/Ghostty-Light.png" />
    <img src="screenshots/Ghostty-Light.png" width="600" alt="Ghostty — Delightful" />
  </picture>
</p>

<h1 align="center">Delightful for Ghostty</h1>

<p align="center">
  Warm, OKLCH-derived color themes for the <a href="https://ghostty.org">Ghostty</a> terminal emulator.
</p>

---

## Install

### Quick (curl)

```bash
mkdir -p ~/.config/ghostty/themes
curl -fsSL https://raw.githubusercontent.com/kylesnav/delightful-ghostty/main/themes/delightful-light -o ~/.config/ghostty/themes/delightful-light
curl -fsSL https://raw.githubusercontent.com/kylesnav/delightful-ghostty/main/themes/delightful-dark -o ~/.config/ghostty/themes/delightful-dark
```

### Manual

```bash
git clone https://github.com/kylesnav/delightful-ghostty.git
mkdir -p ~/.config/ghostty/themes
cp delightful-ghostty/themes/delightful-light delightful-ghostty/themes/delightful-dark ~/.config/ghostty/themes/
```

Then set your theme in `~/.config/ghostty/config`:

```
theme = delightful-light
```

Or `delightful-dark` for dark mode.

## What's Included

- **`themes/delightful-light`** -- Light theme with warm cream background
- **`themes/delightful-dark`** -- Dark theme with warm charcoal background
- **`config`** -- Opinionated Ghostty configuration (fonts, keybinds, window chrome, tmux integration)
- **`shaders/`** -- Optional GLSL post-processing effects (vignette, bloom)

### Config

The included config goes beyond colors -- JetBrains Mono with OpenType features, macOS tab bar, equalized splits (`Cmd+D` / `Cmd+Shift+D`), copy-on-select, and 10M scrollback. This is opinionated and personal; the themes work independently without it.

```bash
cp config ~/.config/ghostty/config
```

### Shaders

Optional GLSL post-processing effects (vignette, bloom):

```bash
# macOS
cp shaders/*.glsl ~/Library/Application\ Support/com.mitchellh.ghostty/shaders/

# Linux
cp shaders/*.glsl ~/.config/ghostty/shaders/
```

Uncomment the `custom-shader` lines in your config to enable.

## Color Mapping

All colors map to [Delightful Design System](https://github.com/kylesnav/delightful-design-system) tokens. Blue slots use the cyan hue at different lightness levels since Delightful has no dedicated blue.

<details>
<summary><strong>Full token mapping</strong></summary>

<br>

| Terminal Color | Design Token | Light | Dark |
|----------------|--------------------------|-----------|-----------|
| Background | bg-page | `#fdf8f3` | `#1e1a16` |
| Foreground | text-primary | `#1b150f` | `#eee9e3` |
| Cursor | accent-primary (pink) | `#f600a3` | `#ff4fa8` |
| Selection BG | accent-primary-subtle | `#ffe6f4` | `#3d2235` |
| Black | neutral-950 | `#16100c` | `#1e1a16` |
| Red | red-400 | `#ed324b` | `#e8554c` |
| Green | green-400 | `#22a448` | `#3aad5f` |
| Yellow | gold-500 | `#c67e00` | `#f5c526` |
| Blue | cyan-400 | `#00a6c0` | `#00a6c0` |
| Magenta | pink-400 | `#f600a3` | `#ff4fa8` |
| Cyan | cyan-300 | `#17c0d6` | `#5cb8d6` |
| White | neutral-100 | `#f6f1eb` | `#eee9e3` |

</details>

## Part of Delightful

This theme is part of the [Delightful Design System](https://github.com/kylesnav/delightful-design-system) -- a warm, neo-brutalist design system built on OKLCH color science.

Other terminal ports:

- [delightful-starship](https://github.com/kylesnav/delightful-starship) -- Starship prompt theme
- [delightful-shell](https://github.com/kylesnav/delightful-shell) -- tmux, zsh config, and terminal utilities
- [delightful-iterm2](https://github.com/kylesnav/delightful-iterm2) -- iTerm2 color profiles

## License

[MIT](LICENSE)
