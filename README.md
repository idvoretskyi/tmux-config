# Tmux Powerline Configuration

[![CI / Tmux Lint](https://github.com/idvoretskyi/tmux-config/actions/workflows/tmux-lint.yml/badge.svg?branch=main)](https://github.com/idvoretskyi/tmux-config/actions/workflows/tmux-lint.yml)
[![Security / Gitleaks](https://github.com/idvoretskyi/tmux-config/actions/workflows/gitleaks.yml/badge.svg?branch=main)](https://github.com/idvoretskyi/tmux-config/actions/workflows/gitleaks.yml)
[![Security / Scorecards](https://github.com/idvoretskyi/tmux-config/actions/workflows/scorecards.yml/badge.svg?branch=main)](https://github.com/idvoretskyi/tmux-config/actions/workflows/scorecards.yml)
[![Security / Dependency Review](https://github.com/idvoretskyi/tmux-config/actions/workflows/dependency-review.yml/badge.svg?branch=main)](https://github.com/idvoretskyi/tmux-config/actions/workflows/dependency-review.yml)

A modern, lightweight tmux configuration with powerline-style theming and Nord color scheme.

## Features

- **Powerline-style status bar** with clean segments and separators
- **Nord color scheme** for a modern, easy-on-the-eyes appearance
- **Improved key bindings** with vim-style navigation
- **Mouse support** enabled
- **True color support** for modern terminals
- **Performance optimized** settings

## Key Bindings

### Prefix Key
- Changed from `Ctrl-b` to `Ctrl-a` (more ergonomic)

### Pane Management
- `Prefix + |` - Split horizontally
- `Prefix + -` - Split vertically
- `Alt + Arrow Keys` - Navigate panes (no prefix needed)
- `Prefix + h/j/k/l` - Vim-style pane navigation
- `Prefix + H/J/K/L` - Resize panes

### Window Management
- `Alt + 1-5` - Quick window selection (no prefix needed)
- `Prefix + c` - New window in current path

### Other
- `Prefix + r` - Reload configuration
- Copy mode uses vi key bindings

## Installation

1. Copy the configuration to your home directory:
   ```bash
   cp .tmux.conf ~/.tmux.conf
   ```

2. Reload tmux configuration:
   ```bash
   tmux source-file ~/.tmux.conf
   ```

3. Or restart tmux for full effect

## Status Bar Layout

```
[Session Name] │ Window1 │ ►Window2◄ │ Window3               15:30 │ 15-Aug │ hostname
```

The status bar includes:
- **Left**: Current session name with powerline styling
- **Center**: Window list with active window highlighted
- **Right**: Time, date, and hostname in powerline segments

## Customization

The configuration uses Nord color scheme variables that can be easily modified. Key color variables are defined at the top of the styling section.

## Requirements

- tmux 2.9+ (for true color support)
- A terminal with 256 color support
- Nerd Fonts or powerline fonts for best appearance (optional)

Enjoy your enhanced tmux experience! 🚀

## Maintainer

Maintained by Ihor Dvoretskyi (@idvoretskyi) — ihor@linux.com