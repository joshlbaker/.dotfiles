### Set up a new machine

1. Install Apple's CLI 

```bash
xcode-select --install
```

2. Clone repo into new hidden directory

```bash
git clone git@github.com:joshlbaker/.dotfiles.git ~/.dotfiles
```

3. Create symlinks

```bash
ln -s ~/.dotfiles/.zshrc ~/.zshrc
ln -s ~/.dotfiles/.gitconfig ~/.gitconfig
ln -s ~/.dotfiles/.p10k.zsh ~/.p10k.zsh
ln -s ~/.dotfiles/custom-colors.iterm-colors ~/Documents/custom-colors.iterm-colors
```

4. Install Homebrew and packages

```bash
# Install Homebrew
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

# Install Homebrew packages
brew bundle --file ~/.dotfiles/Brewfile
```

5. Install NVM

```bash
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash
```

### TODO
- Automate the install scripts
- Organize configs into separate directories + files
