# Setup Linux (Rocky)

In just a few easy steps! Kidding. Never easy enough, but not too bad either.

## Homebrew

First, install Homebrew.

```console
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

## Oh My Zsh

Second, install Oh My ZSH.

```console
sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

## Python

Third, install Python with Homebrew via pipx dependency and use pipx to install dotfiles and checkoutmanager.

```console
brew install pipx
.local/bin/pipx install dotfiles
.local/bin/pipx install checkoutmanager
```

## Firefox

- [Bitwarden Password Manager Add-On](https://addons.mozilla.org/en-US/firefox/addon/bitwarden-password-manager/)
- [Gnome Shell Integration](https://addons.mozilla.org/en-US/firefox/addon/gnome-shell-integration/)
- [React Developer Tools](https://addons.mozilla.org/en-US/firefox/addon/react-devtools/)

## Dotfiles

Requires dotfiles and [GitHub Personal access token](https://github.com/settings/tokens)

```console
sh -c "$(curl -fsSL https://raw.githubusercontent.com/aclark4life/setup-linux/main/dotfiles.sh)"
```

## Everything Else

Just a few more steps! Not really, but hang in there.

### Settings

#### Terminal

- Preferences → Profiles → Unnamed → ☑︎ Custom font → Monospace → 16


