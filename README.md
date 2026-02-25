# tmux Configuration

tmux configuration with true color support, vi-style keybindings, and a clean status bar.

## Features

- **General**: Non-login shell (prevents duplicate PATH), scrollback buffer 10000 lines, reduced Escape delay, focus events enabled, system clipboard integration
- **UI**: True color (24-bit) support, mouse enabled, windows/panes numbered from 1, automatic window renaming
- **Keybindings**: `C-a` prefix, vi-style copy mode, vim-style pane navigation/resizing, config reload, current path preserved on split
- **Statusline**: Session name (left), date/time/hostname (right), cyan-highlighted active window

## Keybindings

| Key                  | Action                              |
| -------------------- | ----------------------------------- |
| `C-a`                | Prefix key                          |
| `prefix` + `r`       | Reload configuration                |
| `prefix` + `-`       | Split pane vertically               |
| `prefix` + `\`       | Split pane horizontally             |
| `prefix` + `Tab`      | Switch to last active window        |
| `prefix` + `Shift+Tab` | Switch to last active session      |
| `prefix` + `h/j/k/l` | Navigate panes (left/down/up/right) |
| `prefix` + `H/J/K/L` | Resize panes (left/down/up/right)   |
| `Escape` (copy mode) | Cancel copy mode                    |
| `v` (copy mode)      | Begin selection                     |
| `y` (copy mode)      | Yank to system clipboard            |

## Installation

```bash
ln -sf $(pwd)/tmux.conf ~/.tmux.conf
tmux source-file ~/.tmux.conf
```

## License

This project is licensed under the terms of the [MIT License](LICENSE).
