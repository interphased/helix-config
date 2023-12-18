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
npm install -g vscode-langservers-extracted typescript-language-server typescript eslint prettier
```
