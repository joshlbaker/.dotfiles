### Set up a new machine

1. Install Apple's CLI 

```
xcode-select --install
```

2. Clone repo into new hidden directory

```
git clone git@github.com:joshlbaker/.dotfiles.git ~/.dotfiles
```

3. Create symlinks

```
ln -s ~/.dotfiles/.zshrc ~/.zshrc
ln -s ~/.dotfiles/.gitconfig ~/.gitconfig
ln -s ~/.dotfiles/.p10k.zsh ~/.p10k.zsh
ln -s ~/.dotfiles/custom-colors.iterm-colors ~/Documents/custom-colors.iterm-colors
```

4. Install Homebrew and packages

```
# Install Homebrew
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

# Install Homebrew packages
brew bundle --file ~/.dotfiles/Brewfile
```

### TODO
- Automate the install scripts
- Organize configs into separate directories + files
