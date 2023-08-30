---
date: 2023-08-30
author: Mikey Garcia, @gikeymarcia
title: Tmux Configuration
---

Contains configuration and supporting scripts for `tmux`.

### Installation

**Requirements:**

- `tmux`
- `git`

These commands will install this tmux configuration and the necessary plugins at `~/.config/tmux/`.

```bash
git clone URL ~/.config/tmux
~/.config/tmux/scripts/tmux-kickstart.sh

# highly recommended add to your .bashrc/.zshrc
alias t=~/.config/tmux/scripts/tmux-quick-launcher.sh
```

### Features

- vim-based remaps
- `<C-a>` is the prefix key
- alt+vim directions (`h j k l`) to change panes
- new splits & windows created with `c % "` are at current working directory
- Prefix alt-`c % "` to use default pane opening rules
- status bar is stylized and on top
- copy mode uses vim keys
- reload `tmux.conf` with prefix `N`
- `tmux-quick-launcher.sh` to easily change/create sessions (requires `fzf`)
