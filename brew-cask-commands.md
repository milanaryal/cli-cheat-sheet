# brew-cask-commands

#### Search

```zsh
brew search text
```

Search for formulas and casks.

#### Information

```zsh
brew info cask_name
```
Display information about a given cask.

#### Install Cask

```zsh
brew install --cask cask_name
```

A command that installs App on your Mac using Homebrew Cask.

#### Uninstall Cask

```zsh
brew uninstall --cask cask_name
```

A command that uninstalls App on your Mac using Homebrew Cask. The `--cask` flag is used to specify that the package being uninstalled is a cask.

```zsh
brew uninstall --cask --zap cask_name
```

The `--zap` flag is used to remove all files associated with the package being uninstalled.

```zsh
brew uninstall --cask --zap --force cask_name
```

The `--force` flag is used to force the uninstallation of the package.


_Further resources: [tldr brew --cask](https://tldr.inbrowser.app/pages/common/brew-cask)._
