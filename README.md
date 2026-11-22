# my-zsh
Installation Guide for my Z-Shell setup, including oh-my-zsh, themes, auto-completion for various tools (I use), neovim and some faster alternatives to built-ins.

| :exclamation:  At the moment the playbook is extremely intrusive and deletes a bunch of stuff. If you want to migrate from your current setup or merge, I highly recommend to first make a back up or merge manually. |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

## Installation

Just run `ansible-playbook -i inventory playbook.yaml -K` in this folder.

## Deletes resources

In the feature I want to gracefully upgrade the environment, but at the moment it always creates a new one. In the process a bunch of resources are deleted.

- ${HOME}/.zshrc
- ${HOME}/.oh-my-zsh
- ${HOME}/.local/share/fonts/Meslo
- /opt/nvim

## ToDo

- Gracefully Upgrade
- Nvim Setup
- Extensions
