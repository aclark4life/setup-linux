# Setup Linux

In just a few easy steps!

Kidding.

Never easy enough, but not too bad either.

## Prerequisites

### Debian 11

Install Debian 11 via DVD.

### APT

Update `/etc/apt/sources.list`.

```
deb http://deb.debian.org/debian/ bullseye main contrib non-free
deb http://security.debian.org/ bullseye-security main contrib
deb http://deb.debian.org/debian/ bullseye-updates main contrib non-free
deb http://deb.debian.org/debian/ bullseye-backports main contrib non-free
```

Install additional packages.

```
apt update
apt install -y build-essential curl fortune linux-image-5.16.0-0.bpo.3-amd64 neovim python3-pip python3-venv task-kde-desktop zsh
```

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

Third, install `pipx`.

```console
pip3 install pipx
pipx install dotfiles
pipx install checkoutmanager
```

## Everything Else

Just a few more steps! Hang in there.

### Firefox + LastPass

Install the Firefox [LastPass Password Manager Add-On](https://addons.mozilla.org/en-US/firefox/addon/lastpass-password-manager). 

### Dotfiles

Requires [dotfiles](https://pypi.org/project/dotfiles) and GitHub Personal access token from [GitHub → Settings → Developer settings → Personal access tokens](https://github.com/settings/tokens).

```console
sh -c "$(curl -fsSL https://raw.githubusercontent.com/aclark4life/setup-linux/main/dotfiles.sh)"
```

### Developer

Update dotfiles and repositories defined in [.checkoutmanager.cfg](https://github.com/reinout/checkoutmanager/blob/master/checkoutmanager/sample.cfg) via ``up`` alias.

![screenshot](screenshot.png)

```console
up
```

#### Postgresql

```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/aclark4life/setup-linux/main/postgresql.sh)"
```

#### Node

```
brew install nvm
nvm install 14
nvm use 14
```

#### GitHub

```
brew install gh
```

## More Steps

OK, I lied! More steps.

### Audio

Add kernel configuration (via https://github.com/Focusrite-Scarlett-on-Linux/sound-usb-kernel-module)

```
echo "options snd_usb_audio vid=0x1235 pid=0x8212 device_setup=1" > /etc/modprobe.d/scarlett.conf
```
