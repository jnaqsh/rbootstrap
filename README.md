# rBootstrap v3.0.0

rBootstrap is the RTL version of [Twitter Bootstrap](http://getbootstrap.com).

## Bugs

Have a bug or a feature request? [Please open a new issue](https://github.com/jnaqsh/rbootstrap/issues).


## Documentation

Bootstrap's documentation, included in this repo in the root directory, is built with [Jekyll](http://jekyllrb.com) and publicly hosted on GitHub Pages at [http://rbootstrap.ir](http://rbootstrap.ir). The docs may also be run locally.

### Running documentation locally

1. If necessary, [install Jekyll](http://jekyllrb.com/docs/installation) (requires v1.x).
2. From the root `/rbootstrap` directory, run `jekyll serve` in the command line.
  - **Windows users:** run `chcp 65001` first to change the command prompt's character encoding ([code page](http://en.wikipedia.org/wiki/Windows_code_page)) to UTF-8 so Jekyll runs without errors.
3. Open [http://localhost:9001](http://localhost:9001) in your browser, and voilà.

Learn more about using Jekyll by reading their [documentation](http://jekyllrb.com/docs/home/).

### Documentation for previous releases

Documentation for v2.3.2 has been made available for the time being at [http://rbootstrap.ir/2.3.2/](http://rbootstrap.ir/2.3.2/) while folks transition to Bootstrap 3.



## Compiling CSS and JavaScript

Bootstrap uses [Grunt](http://gruntjs.com/) with convenient methods for working with the framework. It's how we compile our code, run tests, and more. To use it, install the required dependencies as directed and then run some Grunt commands.

### Install Grunt

From the command line:

1. Install `grunt-cli` globally with `npm install -g grunt-cli`.
2. Install the [necessary local dependencies](package.json) via `npm install`

When completed, you'll be able to run the various Grunt commands provided from the command line.

**Unfamiliar with `npm`? Don't have node installed?** That's a-okay. npm stands for [node packaged modules](http://npmjs.org/) and is a way to manage development dependencies through node.js. [Download and install node.js](http://nodejs.org/download/) before proceeding.

### Available Grunt commands

#### Build - `grunt`
Run `grunt` to run tests locally and compile the CSS and JavaScript into `/dist`. **Requires recess and uglify-js.**

#### Only compile CSS and JavaScript - `grunt dist`
`grunt dist` creates the `/dist` directory with compiled files. **Requires recess and uglify-js.**

#### Tests - `grunt test`
Runs jshint and qunit tests headlessly in [phantomjs](http://code.google.com/p/phantomjs/) (used for ci). **Requires phantomjs.**

#### Watch - `grunt watch`
This is a convenience method for watching just Less files and automatically building them whenever you save.

### Troubleshooting dependencies

Should you encounter problems with installing dependencies or running Grunt commands, uninstall all previous dependency versions (global and local). Then, rerun `npm install`.



## Versioning

For transparency and insight into our release cycle, and for striving to maintain backward compatibility, Bootstrap will be maintained under the Semantic Versioning guidelines as much as possible.

Releases will be numbered with the following format:

`<major>.<minor>.<patch>`

And constructed with the following guidelines:

* Breaking backward compatibility bumps the major (and resets the minor and patch)
* New additions without breaking backward compatibility bumps the minor (and resets the patch)
* Bug fixes and misc changes bumps the patch

For more information on SemVer, please visit [http://semver.org/](http://semver.org/).



## Authors

**Hamed Ramezanian**

+ [http://twitter.com/iceage2098](http://twitter.com/iceage2098)
+ [http://github.com/iCEAGE](http://github.com/iCEAGE)



## Copyright and license

[the Apache 2.0 license](LICENSE).
