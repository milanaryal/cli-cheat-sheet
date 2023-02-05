## Homebrew cheatsheet

### Commands

`brew install git` - Install a package
`brew uninstall git` - Remove/Uninstall a package
`brew upgrade git` - Upgrade a package
`brew unlink git` - Unlink
`brew link git` - Link
`brew switch git 2.5.0` - Change versions
`brew list --versions git` - See what versions you have

### More package commands

`brew info git` - List versions, caveats, etc
`brew cleanup git` - Remove old versions
`brew edit git` - Edit this formula
`brew cat git` - Print this formula
`brew home git` - Open homepage
`brew search git` - Search for formulas

### Global commands

`brew update` - Update brew and cask
`brew upgrade` - Upgrade all packages
`brew list` - List installed
`brew outdated` - What’s due for upgrades?
`brew doctor` - Diagnose brew issues

### Brew Cask commands

`brew install --cask firefox` - Install the Firefox browser
`brew list --cask` - List installed applications
`brew uninstall firefox`
`brew uninstall --cask --zap --force firefox`

> Cask commands are used for interacting with graphical applications.

_Ref. <https://devhints.io/homebrew>_

```zh
Brew cask

Example usage:
  brew search TEXT|/REGEX/
  brew info [FORMULA|CASK...]
  brew install FORMULA|CASK...
  brew update
  brew upgrade [FORMULA|CASK...]
  brew uninstall FORMULA|CASK...
  brew list [FORMULA|CASK...]

Troubleshooting:
  brew config
  brew doctor
  brew install --verbose --debug FORMULA|CASK

brew list
brew upgrade
brew tap homebrew/cask

brew install --cask appcleaner
brew install --cask maintenance

brew install --cask anydesk
brew install --cask dropbox
brew install --cask gimp
brew install --cask google-chrome
brew install --cask google-drive
brew install --cask iina
brew install --cask transmission
brew install --cask visual-studio-code
brew install --cask microsoft-edge
brew install --cask micro soft-office

brew tap homebrew/cask-versions
brew install --cask transmission-beta
i.e., brew install --cask homebrew/cask-versions/transmission-beta

brew uninstall --cask --zap --force google-chrome
brew uninstall --cask --zap --force visual-studio-code
brew uninstall --cask --zap --force microsoft-auto-update
brew uninstall --cask --zap --force microsoft-edge
brew uninstall --cask --zap --force microsoft-office
```
