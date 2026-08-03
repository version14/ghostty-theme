# Version 14 Theme for Ghostty

A terminal color scheme for [Ghostty](https://ghostty.org), built around the Version 14 brand palette, the same palette used across the [Zed](https://github.com/version14/zed-theme), [VS Code](https://github.com/version14/vscode-theme), and [Neovim/Vim](https://github.com/version14/nvim-theme) ports.

## Variants

| Variant | File | Description |
|---|---|---|
| **Version 14** | `version14` | Deep dark background with a violet accent |
| **Version 14 Black** | `version14-black` | Pure black background, for OLED displays |
| **Version 14 Light** | `version14-light` | Bright neutral surfaces with a deep violet accent |

> The violet accent is a placeholder hue. It replaces a retired lime green accent and will change again once a permanent hue is chosen. The rest of the palette is stable.

## Installation

1. Copy the variant file you want into `~/.config/ghostty/themes/`.

   One file at a time:
   ```sh
   curl -o ~/.config/ghostty/themes/version14 \
     https://raw.githubusercontent.com/version14/ghostty-theme/main/version14
   ```

   Or all three at once:
   ```sh
   git clone https://github.com/version14/ghostty-theme /tmp/ghostty-theme
   cp /tmp/ghostty-theme/version14* ~/.config/ghostty/themes/
   ```

2. In `~/.config/ghostty/config`, set:
   ```
   theme = version14
   ```

3. Reload Ghostty's config (`Cmd+Shift+,` or restart) to apply.

Repeat step 2 with `version14-black` or `version14-light` to switch variants.

## Verify

```sh
ghostty +show-config | grep '^theme'
```

This should print `theme = version14` (or whichever variant you set). If it does not, confirm the file landed in `~/.config/ghostty/themes/` and that `config` was saved before reloading.

## Color Palette

### Version 14 (Dark)

| Role | Color |
|---|---|
| Background | `#14171B` |
| Foreground | `#F2F4F6` |
| Accent (placeholder) | `#B7A2FF` |
| Red | `#FF5C59` |
| Green | `#4BDE7F` |
| Yellow | `#FFA85E` |
| Blue | `#78AFFF` |
| Magenta | `#ED8EF3` |
| Cyan | `#B7A2FF` |

### Version 14 Black

| Role | Color |
|---|---|
| Background | `#000000` |
| Foreground | `#F2F4F6` |
| Accent (placeholder) | `#B7A2FF` |
| Red | `#FF5C59` |
| Green | `#4BDE7F` |
| Yellow | `#FFA85E` |
| Blue | `#78AFFF` |
| Magenta | `#ED8EF3` |
| Cyan | `#B7A2FF` |

### Version 14 Light

| Role | Color |
|---|---|
| Background | `#EBEDEF` |
| Foreground | `#0D0F11` |
| Accent (placeholder) | `#5F3BBB` |
| Red | `#B91A25` |
| Green | `#166534` |
| Yellow | `#8F4400` |
| Blue | `#0054CB` |
| Magenta | `#8C2293` |
| Cyan | `#5F3BBB` |

## Also available for

- [Zed](https://github.com/version14/zed-theme)
- [VS Code](https://github.com/version14/vscode-theme)
- [Neovim](https://github.com/version14/nvim-theme)
- [Vim](https://github.com/version14/vim-theme)
- [Starship](https://github.com/version14/starship-theme)
- [gh-dash](https://github.com/version14/gh-dash-theme)
- [Atuin](https://github.com/version14/atuin-theme)

## License

[MIT](./LICENSE) © [Mathieu Souflis](https://mathieusouflis.fr)
