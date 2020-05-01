How to
=====

## [clear Git cache](https://stackoverflow.com/questions/25436312/gitignore-not-working/25436481)

```bash
$ git rm -rf --cached .
```

## clean `node_modules` folder of packages that are not in `package.json`?

```bash
$ npm prune [<name> [<name ...]]
```

This command removes "extraneous" packages. If a package name is provided, then only packages matching one of the supplied names are removed.

Extraneous packages are packages that are not listed on the parent package's dependencies list.

## delete `node_modules` folder on Windows machine?

Due to its folder nesting Windows can't delete the folder as its name is too long. To solve this, install [RimRaf](https://github.com/isaacs/rimraf):

```bash
$ npm install rimraf -g
```

And in the project folder delete the `node_modules` folder with:

```bash
$ rimraf node_modules
```
