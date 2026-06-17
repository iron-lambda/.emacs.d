# .emacs.d

![Language](https://img.shields.io/badge/language-Emacs_Lisp-7F5AB6)
[![License: MIT](https://img.shields.io/badge/license-MIT-green)](LICENSE)

A minimal Emacs configuration tailored for Racket development. Built on `use-package` with a focus on simplicity — no bloated frameworks, just the essentials for a clean and productive editing experience.

## Features

- **Racket IDE** — `racket-mode` with REPL integration, XP mode (auto-completion), and paredit for structural editing
- **Clean UI** — no toolbar, no scrollbar, no startup screen
- **Modern defaults** — bar cursor, line numbers, electric pairs, rainbow parentheses
- **Which-key** — discoverable keybindings with on-screen hints
- **Comment toggle** — `C-c c` to comment/uncomment regions

## Packages

| Package | Purpose |
|---------|---------|
| `racket-mode` | Racket major mode with REPL (`C-c C-r` send region, `C-c C-z` open REPL) |
| `racket-xp` | Auto-completion and inline error checking |
| `paredit` | Structural editing for S-expressions |
| `which-key` | Interactive keybinding discovery |

## Installation

1. Clone this repository to `~/.emacs.d`:

```bash
git clone https://github.com/iron-lambda/.emacs.d.git ~/.emacs.d
```

2. Launch Emacs. Packages are installed automatically on first run.

## Key Bindings

| Shortcut | Action |
|----------|--------|
| `C-c c` | Comment/uncomment region |
| `C-c C-r` | Send region to Racket REPL |
| `C-c C-z` | Open Racket REPL |

## Customization

This config uses the Tsinghua MELPA mirror for faster downloads in China. To switch to the official mirror, edit the `package-archives` in `init.el`:

```elisp
(setq package-archives
      '(("melpa" . "https://melpa.org/packages/")
        ("gnu"   . "https://elpa.gnu.org/packages/")))
```

## Requirements

- Emacs 27+ (tested with Emacs 29)
- Internet connection (for initial package installation)

## License

[MIT](LICENSE)
