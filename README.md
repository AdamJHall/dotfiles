# Dotfiles

Personal dotfiles managed with [chezmoi](https://www.chezmoi.io/).

## Setup

```sh
chezmoi init --apply https://github.com/adamhall1992/dotfiles
```

## Dependencies

### Terminal — [Alacritty](https://alacritty.org/)

**Font:** [UbuntuMono Nerd Font Mono](https://www.nerdfonts.com/font-downloads)

---

### Multiplexer — [tmux](https://github.com/tmux/tmux)

**Plugin manager:** [TPM](https://github.com/tmux-plugins/tpm)

**Catppuccin theme** must be cloned manually (so its color variables are available before TPM initializes) into `~/.config/tmux/plugins/tmux/`:

```sh
git clone https://github.com/catppuccin/tmux ~/.config/tmux/plugins/tmux
```

After launching tmux, install the remaining plugins with `prefix + I`:

| Plugin | Purpose |
|--------|---------|
| [tmux-sensible](https://github.com/tmux-plugins/tmux-sensible) | Sensible defaults |
| [tmux-autoreload](https://github.com/b0o/tmux-autoreload) | Auto-reload config on save |
| [tmux-fzf](https://github.com/sainnhe/tmux-fzf) | fzf integration in tmux |
| [tmux-better-mouse-mode](https://github.com/nhdaly/tmux-better-mouse-mode) | Improved mouse scrolling |
| [tmux-cpu](https://github.com/tmux-plugins/tmux-cpu) | CPU/memory status widgets |

**Clipboard:** [wl-clipboard](https://github.com/bugaevc/wl-clipboard) — required for the pane copy menu (Wayland).

---

### Shell — [zsh](https://www.zsh.org/) + [oh-my-zsh](https://ohmyz.sh/) + [fzf](https://github.com/junegunn/fzf)

**oh-my-zsh plugins** (see each repo for install instructions — clone into `~/.oh-my-zsh/custom/plugins/`):

| Plugin | Purpose |
|--------|---------|
| [fzf-tab](https://github.com/Aloxaf/fzf-tab) | fzf-powered tab completion |
| [zsh-autosuggestions](https://github.com/zsh-users/zsh-autosuggestions) | Fish-style inline suggestions |
| [zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting) | Command syntax highlighting |
| [zsh-fzf-history-search](https://github.com/joshskidmore/zsh-fzf-history-search) | fzf history search |
| [zsh-completions](https://github.com/zsh-users/zsh-completions) | Extra completion definitions |

**[Catppuccin zsh-syntax-highlighting theme](https://github.com/catppuccin/zsh-syntax-highlighting)** — must be cloned into `~/.oh-my-zsh/custom/plugins/zsh-syntax-highlighting-catppuccin/`:

```sh
git clone https://github.com/catppuccin/zsh-syntax-highlighting ~/.oh-my-zsh/custom/plugins/zsh-syntax-highlighting-catppuccin
```

---

### Prompt — [Starship](https://starship.rs/)

---

### Node — [NVM](https://github.com/nvm-sh/nvm)
