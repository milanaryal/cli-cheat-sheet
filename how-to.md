How to
=======

## How to clean `node_modules` folder of packages that are not in `package.json`?

`npm prune [<name> [<name ...]]`

This command removes "extraneous" packages. If a package name is provided, then only packages matching one of the supplied names are removed.

Extraneous packages are packages that are not listed on the parent package's dependencies list.

## How to delete `node_modules` folder on Windows machine?

Due to its folder nesting Windows can't delete the folder as its name is too long. To solve this, install [RimRaf](https://github.com/isaacs/rimraf):

`npm install rimraf -g`

And in the project folder delete the `node_modules` folder with:

`rimraf node_modules`
