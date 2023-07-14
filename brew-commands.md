# brew-commands

_[tldr brew](https://tldr.inbrowser.app/pages/common/brew),_ & _[Homebrew cheatsheet](https://devhints.io/homebrew) by devhints.io._

Using homebrew you can install and manage packages of different services and modules. You can start and stop a service directly from brew and use the service efficiently.

#### List all packages installed using brew

```zsh
brew list
```

The above command will list down all the packages installed via brew on your system.

#### List down all services running using brew

```zsh
brew services list
```

This command will list all services started using brew.

#### Install a Package using brew

```zsh
brew install package_name
```

To install a package using homebrew we can use the above command. You need to add the package name after brew install command to install a new package.

#### Uninstall or remove a package in Homebrew

```zsh
brew uninstall package_name
```

Like installation command, you can use uninstall in place of install to completely remove a package from homebrew.

```zsh
brew uninstall --force package_name
```

The `--force` or `-f` flag is used to remove package even if it has dependencies.

#### Upgrade a package using Homebrew

```zsh
brew upgrade package_name
```

To upgrade a package to its latest version in Homebrew, you can use above command. I will upgrade the package.

#### Link/Unlink a package in Homebrew

```zsh
# To unlink a package
brew unlink package_name

# To link a package
brew link package_name
```

To unlink a package you can run command `brew unlink package_name`. This will not remove the package from your system but if you want to use the package, you will need to link them using `brew link package_name` commad.

#### Change to specific version of a package

```zsh
brew switch package_name 2.1.5
```

If you are using multiple versions of a package in Homebrew, you can switch to specific version using above command.

#### Check version of a package in Homebrew

```zsh
brew list --versions package_name
```

To check the versions of a package installed via Homebrew, you can use the command `brew list --versions package_name`. It will print the version in the terminal window.

#### Remove old version of a package

```zsh
brew cleanup package_name
```

If you want to remove the old versions of a package, you can use the above command in the terminal with brew installed.

```zsh
brew cleanup
```

A command that frees up space on your Mac by removing old versions of formulae and small kegs of data. It also deletes old downloads from the Homebrew download-cache.

#### Open home page of a package in browser

```zsh
brew home package_name
```

To open the homepage of a package in the browser, you can use the brew home command. For example, if you want to open the homepage of Git package installed via homebrew, you can use the command - `brew home git`.

#### Update Homebrew

```zsh
brew update
```

To update the Homebrew version on your local system you can use the above command. The command will install components and modules that are required to update the Homebrew version.

#### Update all packages installed via Homebrew

```zsh
brew upgrade
```

The command can be used to upgrade all the packages and modules installed via Homebrew.

```zsh
brew outdated
```
The command will show the list of Homebrew packages that are not updated to its latest version.

#### Check any issue occurred in brew or packages

```zsh
brew doctor
```

If you are facing any error in Homebrew or its packages then you can run the above command. It will find the issues and show you the list of issues in the terminal.
