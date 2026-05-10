## Tmux Configuration

![][screenshot]

Configuration and scripts for `tmux` v3.1+ on Linux and MacOSX.

## Features

- Vim-based remaps with stylized status bar up top
- Prefix key set to `<C-a>`
- Reload `tmux.conf` with prefix `R`
- Change active panes with alt+vim directions (`h j k l`)
- New splits & windows created with Prefix + `c % "` are at current working directory
    - Prefix alt-`c % "` to use default pane opening rules
- Copy mode uses vim keys
- `tmux-quick-launcher.sh` to easily change/create sessions
- Prefix `<C-s>` to save your session
- Prefix `<C-r>` to reload your session
- Prefix `p` to toggle synchronized panes (multi-type)
- Prefix `C-t` switch sessions using sesh
- Prefix `C-o` switch to previous session

## Installation

### Quickstart

```bash
git clone https://github.com/gikeymarcia/tmux-config.git ~/.config/tmux
~/.config/tmux/scripts/tmux-kickstart.sh
```

The tmux-kickstart.sh script installs this config and [plugins][tpm] to
`~/.config/tmux/`. If a config is found at '~/.tmux.conf' it is moved to
'~/.tmux.conf.bak'.

### Requirements

- `tmux`
- `git`
- `fzf` (for tmux-quick-launcher.sh)
- [`sesh`](https://github.com/joshmedeski/sesh) (for session switching Prefix C-t)

### Recommended

```bash
# add this alias to your .bashrc/.zshrc
alias t=~/.config/tmux/scripts/tmux-quick-launcher.sh
```

[tpm]: <https://github.com/tmux-plugins/tpm>
"TPM: The Tmux Plugin Manager"
[screenshot]: <./screenshot.png>
"Upper left: Session [pane#] PaneName  ------ Upper Right: Panes, Time"
