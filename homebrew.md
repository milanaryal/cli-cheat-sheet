---
title: "Homebrew"
description: "The missing package manager for macOS"
date: 2023-03-11
---

### Example usage

```sh
brew search <FORMULA|CASK>
brew info <FORMULA|CASK>
brew install <FORMULA|CASK>
brew update
brew upgrade <FORMULA|CASK>
brew uninstall <FORMULA|CASK>
brew list <FORMULA|CASK>
```

### Troubleshooting

```sh
brew config
brew doctor
brew install --verbose --debug <FORMULA|CASK>
```

### Essential CLI based app

[TL;DR](https://tldr.inbrowser.app/pages/common/brew)

```sh
brew install gh
brew install tldr
brew install unar
```

### Essential GUI based app

[TL;DR](https://tldr.inbrowser.app/pages/common/brew-cask)

```sh
brew tap homebrew/cask
```

```sh
brew install --cask android-file-transfer
brew install --cask anydesk
brew install --cask appcleaner
brew install --cask firefox
brew install --cask codeedit
brew install --cask dropbox
brew install --cask gimp
brew install --cask google-chrome
brew install --cask google-drive
brew install --cask iina
brew install --cask maintenance
brew install --cask microsoft-edge
brew install --cask microsoft-office
brew install --cask tor-browser
brew install --cask transmission
brew install --cask visual-studio-code
```

# Install beta version GUI app

```sh
brew tap homebrew/cask-versions
```

```sh
brew install --cask transmission-beta
```

i.e., 

```sh
brew install --cask homebrew/cask-versions/transmission-beta
```

### Uninstall GUI app and related files

```sh
brew uninstall --cask <CASK>
```

```sh
brew uninstall --cask --zap <CASK>
```

i.e.,

```sh
brew uninstall --cask --zap --force visual-studio-code
brew uninstall --cask --zap --force microsoft-auto-update
brew uninstall --cask --zap --force microsoft-edge
brew uninstall --cask --zap --force microsoft-office
```

### Updating and upgrading casks

[Docs](https://github.com/Homebrew/homebrew-cask/blob/master/USAGE.md#updatingupgrading-casks).

```sh
brew upgrade --cask <CASK>
```

```sh
brew upgrade --cask --greedy
```

Alternatively, [`brew cu`](https://github.com/buo/homebrew-cask-upgrade#readme)

```sh
brew cleanup
```
