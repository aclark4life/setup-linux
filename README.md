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

## pipx

Third, install pipx and use it to install dotfiles and checkoutmanager.

```console
brew install pipx
.local/bin/pipx install dotfiles
.local/bin/pipx install checkoutmanager
```

## Firefox

Install extensions.

- [Bitwarden Password Manager Add-On](https://addons.mozilla.org/en-US/firefox/addon/bitwarden-password-manager/)
- [React Developer Tools](https://addons.mozilla.org/en-US/firefox/addon/react-devtools/)

## Dotfiles

Requires dotfiles and [Personal access token](https://github.com/settings/tokens).

```console
sh -c "$(curl -fsSL https://raw.githubusercontent.com/aclark4life/setup-linux/main/dotfiles.sh)"
```

## Everything Else

Just a few more steps! Not really, but hang in there.

### Terminal

- Preferences → Profiles → Unnamed → Text Appearance → ☑︎ Custom font → Monospace → 16
- Preferences → Profiles → Unnamed → Sound → ☐ Terminal bell

### Settings

- Privacy → Screen Lock → ☐ Automatic Screen Lock
- Mouse & Touchpad → ☑︎ Natural Scrolling 
- Mouse & Touchpad → ☑︎ Tap to Click

### Tweaks

- Window Titlebars → Titlebar Buttons → ☑︎ Maximize
- Window Titlebars → Titlebar Buttons → ☑︎ Minimize

### Extensions

- ☑︎ Dash to Dock
- ☑︎ [ArcMenu](https://extensions.gnome.org/extension/3628/arcmenu/)
- ☑︎ [Bing Wallpaper](https://extensions.gnome.org/extension/1262/bing-wallpaper-changer/)
- ☑︎ [Clipboard Indicator](https://extensions.gnome.org/extension/779/clipboard-indicator/)
- ☑︎ [Frippery Move Clock](https://extensions.gnome.org/extension/2/move-clock/)
- ☑︎ [Gnome Shell Integration](https://addons.mozilla.org/en-US/firefox/addon/gnome-shell-integration/)
- ☑︎ [OpenWeather](https://extensions.gnome.org/extension/750/openweather/)
- ☑︎ [Vitals](https://extensions.gnome.org/extension/1460/vitals/)
