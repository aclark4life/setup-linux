# Setup Linux (Debian 12)

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

## Additional packages

Third, install additional packages via apt, brew and pipx.

### apt

```console
sudo apt install -y build-essential \
                    bsdmainutils \
                    curl \
                    nfs-common \
                    python3-pip \
                    python3-venv \
                    pipx \
	            whois \
                    xfishtank \
                    zsh
```


### brew

```console
brew install fortune gh nvm
```

### pipx

```console
pipx install dotfiles
pipx install checkoutmanager
```

## Everything Else

Just a few more steps! Hang in there.

### Dotfiles

Requires [dotfiles](https://pypi.org/project/dotfiles) and GitHub Personal access token from [GitHub → Settings → Developer settings → Personal access tokens](https://github.com/settings/tokens).

```console
sh -c "$(curl -fsSL https://raw.githubusercontent.com/aclark4life/setup-linux/main/dotfiles.sh)"
```

### Firefox

Install add-ons.

- [Bitwarden Password Manager Add-On](https://addons.mozilla.org/en-US/firefox/addon/bitwarden-password-manager/)
- [React Developer Tools](https://addons.mozilla.org/en-US/firefox/addon/react-devtools/).

## Developer

### Postgresql

```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/aclark4life/setup-linux/main/postgresql.sh)"
```

#### Node

```
nvm install 14
nvm use 14
```
