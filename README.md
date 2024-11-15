# my-zsh
Installation Guide for my Z-Shell setup.

<img width="1494" alt="Screenshot 2024-11-12 at 23 13 35" src="https://github.com/user-attachments/assets/fd94c9f5-68f9-4f2d-9f18-5450868166eb">

## Install Zsh

If not already part of your distribution, install Zsh using your package manager.

Run `chsh -s /bin/zsh` to switch your shell permanently.

## Install NerdFonts

Most Themes require [NerdFonts](https://www.nerdfonts.com) to work correctly. I usually use [MesloLG Nerd Font](https://github.com/ryanoasis/nerd-fonts/releases/download/v3.2.1/Meslo.zip). The exactly installation instructions can differ based on your OS and Terminal.

## Install Oh-My-Zsh

To better handle Themes and Upgrades. Just follow [their](https://ohmyz.sh/#install) installation instructions.

## Install PowerLevel10k

The Theme I always use. Again, just follow [their](https://github.com/romkatv/powerlevel10k?tab=readme-ov-file#oh-my-zsh) instructions.

Make sure to restart your Terminal after you've set the Theme and configure it to your heart's content.

## Install Plugins

~~Stolen~~ Inspired by [this](https://gist.github.com/n1snt/454b879b8f0b7995740ae04c5fb5b7df) set of instructions. I am going to copy them in case the link breaks.

<details>
<summary>Commands</summary>

### autosuggesions plugin

```
git clone https://github.com/zsh-users/zsh-autosuggestions.git $ZSH_CUSTOM/plugins/zsh-autosuggestions
```

### zsh-syntax-highlighting plugin
 
```
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git $ZSH_CUSTOM/plugins/zsh-syntax-highlighting
```
	
### zsh-fast-syntax-highlighting plugin
 
```
git clone https://github.com/zdharma-continuum/fast-syntax-highlighting.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/plugins/fast-syntax-highlighting
```
	
### zsh-autocomplete plugin
	
```
git clone --depth 1 -- https://github.com/marlonrichert/zsh-autocomplete.git $ZSH_CUSTOM/plugins/zsh-autocomplete
```
</details>

Enable the plugins using `plugins=(git zsh-autosuggestions zsh-syntax-highlighting zsh-autocomplete web-search dotnet docker)`. This also enables web-search (type `google <searchterm>`), dotnet auto-completion and docker auto-completion.

## Eza

`ls` on steriods. Check your package manager if it is available. Add alias.zsh to your ~/.oh-my-zsh/custom containing

```
alias ll="eza -l -g -a --icons"
alias lt="eza -l -g -a --icons -T"
alias ls="eza --icons"
```

## Neovim

Somtime nano is just not cool enough. WIP
