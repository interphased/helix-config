# Installation

```bash
# Essentials
sudo apt install software-properties-common
sudo apt update

# Helix
sudo add-apt-repository ppa:maveonair/helix-editor
sudo apt update
sudo apt install helix

# Node
curl -L https://bit.ly/n-install | bash
n lts

# Language servers (additional servers: https://github-wiki-see.page/m/helix-editor/helix/wiki/How-to-install-the-default-language-servers)
npm install -g vscode-langservers-extracted typescript-language-server typescript eslint prettier @tailwindcss/language-server @olrtg/emmet-language-server

# Gems
# erb_lint doesn't work great with helix right now, so use a local version of erb-formatter instead
gem install erb-formatter

# Lazygit
LAZYGIT_VERSION=$(curl -s "https://api.github.com/repos/jesseduffield/lazygit/releases/latest" | grep -Po '"tag_name": "v\K[^"]*')
curl -Lo lazygit.tar.gz "https://github.com/jesseduffield/lazygit/releases/latest/download/lazygit_${LAZYGIT_VERSION}_Linux_x86_64.tar.gz"
tar xf lazygit.tar.gz lazygit
sudo install lazygit /usr/local/bin

# Tmux
apt install tmux
git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
tmux source ~/.config/tmux/tmux.conf
[CTRL-B] [I]

# Config goes in ~/
git clone https://github.com/interphased/helix-config
```
