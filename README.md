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
git clone git@github.com:matthiebl/.dotfiles ~/.dotfiles
```

5. Install Brew and Brew dependencies
```zsh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

