# .dotfiles

A collection of dotfiles and configurations I use on macOS.

## Setup

First we have to take care of some things I haven't yet automated.

1.  Install command line tools so we can use `git` and `brew`
```zsh
xcode-select --install
```

2. Setup ssh in order to use git
```zsh
ssh-keygen
# use defualt location, and no passphrase
cat ~/.ssh/id_ed25519.pub
```

3. Copy the key into Github [Settings > SSH and GPG keys > New SSH Key](https://github.com/settings/ssh/new)

4. Clone the dotfiles repo
```zsh
git clone git@github.com:matthiebl/.dotfiles.git ~/.dotfiles
```

5. Install Brew and Brew dependencies
```zsh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

## Install

I plan to setup the following with an automated install, but have not gotten around to it yet.

```zsh
brew install --cask iterm2
brew install tmux
brew install neovim
```

Install ohmyzsh
```zsh
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
```

Install Powerlevel10k and the [Meslo Nerd font](https://github.com/romkatv/powerlevel10k?tab=readme-ov-file#meslo-nerd-font-patched-for-powerlevel10k)
```zsh
git clone --depth=1 https://github.com/romkatv/powerlevel10k.git "${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k"
```

## Other

```
brew install choose-gui
```

