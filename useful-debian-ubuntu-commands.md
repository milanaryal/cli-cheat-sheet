## Essential apt commands

Update OS packages: `sudo apt update -y && sudo apt upgrade -y`

To install package: `sudo apt install -y <package_name>`

To search package: `apt search <package_name>`

To know the package version before install: `apt policy <package_name>`

To know the package details: `apt show <package_name>`

To delete package and its dependecies: `apt --purge remove <package_name>`

Add repo: `sudo apt-add-repository <ppa: repo_name> && apt update`

Remove repo: `udo apt-add-repository -r <ppa: repo_name> && apt update`

## Useful Debian/Ubuntu commands

List all packages: `apt list` && `apt list | more` && `apt list | grep foo`

List installed packages: `apt list --installed` && `apt list --installed | grep {pkgNameHere}`

List installed upgradable packages: `apt list --upgradable`

List package dependency: `apt depends {pkgNameHere}` eg. `apt depends sudo`

How do I performs recursive dependency listings similar to apt-cache? `apt rdepends {pkgNames}` eg. `apt rdepends sudo`

How do I hold a package? Package holding means it can not be upgraded till you run unhold on it again. The syntax is: `apt hold {pkgName}` eg. `apt hold sudo`

How do I unhold a package? `apt unhold {pkgName}` eg. `apt unhold sudo`

Search for packages: `apt search <search_term>` or `apt-cache search <search_term>`

See policy of apt package: `apt list -a {pkgNameHere}` eg. `apt list -a sudo` or `apt policy <package_name>` or `apt-cache policy <package_name>`

Show detail info for packages: `apt show <search_term>` or `apt-cache show <search_term>`

Install package: `sudo apt install -y <package_name>` or `sudo apt-get install -y <package_name>`

Remove the binary files of a package: `apt remove <package_name>` or `apt-get remove <package_name>`

Remove everything related to a package, including its configuration files (purge everything): `apt purge <package_name>` or `apt-get purge <package_name>`

Remove package and everything related to a package: `apt remove --purge <package_name>` or `apt-get remove --purge <package_name>`

The autoremove option to remove packages that were automatically installed to satisfy dependencies for other packages and are now no longer needed as dependencies changed or the package(s) needing them were removed in the meantime: `sudo apt autoremove` && `sudo apt --purge autoremove`

Upgrade all installed packages: `sudo apt upgrade` or `sudo apt-get upgrade`

Upgrade one specific package: `sudo apt upgrade <package_name>` or `sudo apt-get upgrade <package_name>`

Often see update and upgrade together like this: `sudo apt update && sudo apt upgrade -y` or `sudo apt-get update && sudo apt-get upgrade -y`

Upgrade vs dist-upgrade (not recommended on production systems): `sudo apt full-upgrade` or `apt-get dist-upgrade`

Upgrade to the latest version of Ubuntu XX.XX LTS on WSL: `sudo do-release-upgrade -d`

List all services on a Linux system: `service --status-all`

Check what version of Linux kernel your system is running on: `uname -r`

Check what version of Linux system you are running on: `cat /etc/issue` or `cat /etc/os-release` or `lsb_release -a`

Show the current more accurate info about Debian update point releases: `cat /etc/debian_version` or `apt install lsb-release && lsb_release -da`

How do I edit the source information file i.e. /etc/apt/sources.list? `sudo apt edit-sources`

Locate the executable file associated with a given command: `which -a [filename]` eg. `which sh` -> `/usr/bin/sh` or `which -a sh` -> `/usr/bin/sh` `/bin/sh`

## apt command options

From the [apt(8)](https://manpages.debian.org/stretch/apt/apt.8.en.html) command man page:

### How to check `apt` version??

On terminal:

`$ apt`

Results:

`apt <version> <distro_name> (<architecture>)`

For eg. <br />
On Debain `apt 1.8.2.1 (amd64)` <br />
On Ubuntu `apt 2.0.2ubuntu0.1 (amd64)`

Specific demo (on Ubuntu):

```text
apt 2.0.2ubuntu0.1 (amd64)
Usage: apt [options] command

apt is a commandline package manager and provides commands for
searching and managing as well as querying information about packages.
It provides the same functionality as the specialized APT tools,
like apt-get and apt-cache, but enables options more suitable for
interactive use by default.

Most used commands:
  list - list packages based on package names
  search - search in package descriptions
  show - show package details
  install - install packages
  reinstall - reinstall packages
  remove - remove packages
  autoremove - Remove automatically all unused packages
  update - update list of available packages
  upgrade - upgrade the system by installing/upgrading packages
  full-upgrade - upgrade the system by removing/installing/upgrading packages
  edit-sources - edit the source information file
  satisfy - satisfy dependency strings

See apt(8) for more information about the available commands.
Configuration options and syntax is detailed in apt.conf(5).
Information about how to configure sources can be found in sources.list(5).
Package and version choices can be expressed via apt_preferences(5).
Security details are available in apt-secure(8).
                                        This APT has Super Cow Powers.
```

Blog post:
  - [apt v1.0](https://mvogt.wordpress.com/2014/04/04/apt-1-0/)
  - [apt v1.1](https://mvogt.wordpress.com/2015/11/30/apt-1-1-released/)
