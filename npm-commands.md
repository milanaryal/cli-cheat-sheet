npm commands
====

npm is the package manager for JavaScript.

### Resources

* [Getting started with npm](https://docs.npmjs.com/)

Requirements
----

Install [Node.js](https://nodejs.org/en/download/package-manager/) on your machine.


Creating a `package.json` file
----

`npm init` - create `package.json` file initating a command line questionnaire

`npm init --yes` or `npm init -y` - create a `package.json` file and fill in default values

Managing global packages
----

`npm ls -g --depth=0` - list out global installed packages

`npm uninstall -g [<name> [<name ...]]` - uninstall global package(s)

`npm outdated --global` - check for outdated global installed packages

Managing project packages
----

`npm list` or `npm ls` (preferred shorthand) - list out currently installed npm packages

`npm ls --depth=0` - only draws out the top of the dependency tree

`npm install` -  will install both "dependencies" and "devDependencies"

`npm install --production` -  will only install "dependencies"

`npm install --dev` - will only install "devDependencies"

`npm outdated` - check for outdated packages

`npm prune [<name> [<name ...]]` - removes "extraneous" packages

`npm where` - show npm installed path

`npm cache clean` - clean npm cache

`npm run-script <script-name>` or for short `npm run <script-name>` - run scripts from `package.json`

<https://devhints.io/npm>
