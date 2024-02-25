# Install steps

1. PACKAGES. Install the following:
  - neovim
  - tmux
  - oh-my-zsh

2. FONTS - Install MonacoNerdFontMono
  - macOS: just double-click it and it will be added to Font Manager
  - linux: AUR: ttf-monaco-nerd-font-git
    or manually copy to /usr/local/share/fonts (or ~/.local/share/fonts/)

3. ZSH
  - Replace .zshrc with dots/zsh/zshrc. See user configuration section at bottom of zshrc.
  - Copy drootang.zsh-theme to ~/.zsh/themes/drootang.zsh-theme

4. NVIM
  - Copy init.lua into ~/.config/nvim/init.lua
  - Launch nvim and wait for installs to complete
  - Install pythonl-lsp-ruff into the venv created by mason-lspconfig for python-lsp-server (pylsp)
    E.g.,
      ~/.local/share/nvim/mason/packages/python-lsp-server/venv/bin/python3 -m pip install python-lsp-ruff

5. TMUX
  - create ~/.config/tmux/plugins
  - install tmux.conf to ~/.config/tmux/tmux.conf
  - git clone https://github.com/catppuccin/tmux.git ~/.config/tmux/plugins/catppuccin

TODO:
- ruff config (from sjfarm)
- bootstrap.sh script to do everything
