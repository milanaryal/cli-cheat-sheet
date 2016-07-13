Gulp Commands
====

Gulp is not only a weird noise you make when attempting to do something physically demanding, it's also an amazing command line tool that allows you to automate a lot of the tedious duties we need to do as web developers.

### Resources

* [gulpjs.com](http://gulpjs.com/)
* [A cheatsheet for gulp](https://github.com/osscafe/gulp-cheatsheet)
* [Building With Gulp](http://www.smashingmagazine.com/2014/06/11/building-with-gulp/)
* [Read more](https://github.com/gulpjs/gulp/blob/master/docs/README.md#articles)


Requirements
----

Install [Node.js](https://nodejs.org/en/download/package-manager/) on your machine.


Installing Gulp
----

`npm install --global gulp-cli` - A Node NPM command that will install the gulp command line commands to your system.


The Basics
----

`gulp` - Will run the default task set up in your gulpfile.js (same as `gulp default`).

`gulp <taskname>` - Will run a task specified in the gulpfile.js so something like `gulp sass` will run the Sass task once and then exit out.

`gulp watch` - Similarly will continuously watch your directory to dynamically run `watch` tasks (defined in gulpfile.js) as files are modified.
