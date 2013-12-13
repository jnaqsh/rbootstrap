# rBootstrap v3.0.3

rBootstrap is the RTL version of [Twitter Bootstrap](http://getbootstrap.com).

To get started, check out [http://rbootstrap.ir](http://rbootstrap.ir)!



## Quick start

Three quick start options are available:

* [Download the latest release](https://github.com/jnaqsh/rbootstrap/archive/v3.0.3.zip).
* Clone the repo: `git clone https://github.com/jnaqsh/rbootstrap.git`.
* Install with [Bower](http://bower.io): `bower install rbootstrap`.

Read the [Getting Started page](http://rbootstrap.ir/getting-started/) for information on the framework contents, templates and examples, and more.

### What's included

Within the download you'll find the following directories and files, logically grouping common assets and providing both compiled and minified variations. You'll see something like this:

```
bootstrap/
├── css/
│   ├── bootstrap.css
│   ├── bootstrap.min.css
│   ├── bootstrap-theme.css
│   └── bootstrap-theme.min.css
├── js/
│   ├── bootstrap.js
│   └── bootstrap.min.js
└── fonts/
    ├── glyphicons-halflings-regular.eot
    ├── glyphicons-halflings-regular.svg
    ├── glyphicons-halflings-regular.ttf
    └── glyphicons-halflings-regular.woff
```

We provide compiled CSS and JS (`bootstrap.*`), as well as compiled and minified CSS and JS (`bootstrap.min.*`). Fonts from Glyphicons are included, as is the optional Bootstrap theme.



## Bugs and feature requests

Have a bug or a feature request? [Please open a new issue](https://github.com/jnaqsh/rbootstrap/issues).



## Documentation

Bootstrap's documentation, included in this repo in the root directory, is built with [Jekyll](http://jekyllrb.com) and publicly hosted on GitHub Pages at [http://rbootstrap.ir](http://rbootstrap.ir). The docs may also be run locally.

### Running documentation locally

1. If necessary, [install Jekyll](http://jekyllrb.com/docs/installation) (requires v1.x).
  - **Windows users:** read [this unofficial guide](https://github.com/juthilo/run-jekyll-on-windows/) to get Jekyll up and running without problems.
2. From the root `/rbootstrap` directory, run `jekyll serve` in the command line.
  - **Windows users:** For Ruby 2.0.0 run `chcp 65001` first to change the command prompt's character encoding ([code page](http://en.wikipedia.org/wiki/Windows_code_page)) to UTF-8 so Jekyll runs without errors. For Ruby 1.9.3 you can alternatively do `SET LANG=en_EN.UTF-8`. In addition, ensure you have Python installed and added in your `PATH` or the build will fail due to our Pygments dependency.
3. Open <http://localhost:9001> in your browser, and voilà.

Learn more about using Jekyll by reading its [documentation](http://jekyllrb.com/docs/home/).

### Documentation for previous releases

Documentation for v2.3.2 has been made available for the time being at <http://rbootstrap.ir/2.3.2/> while folks transition to Bootstrap 3.

[Previous releases](https://github.com/jnaqsh/rbootstrap/releases) and their documentation are also available for download.



## Compiling CSS and JavaScript

Bootstrap uses [Grunt](http://gruntjs.com/) with convenient methods for working with the framework. It's how we compile our code, run tests, and more. To use it, install the required dependencies as directed and then run some Grunt commands.

### Install Grunt

From the command line:

1. Install `grunt-cli` globally with `npm install -g grunt-cli`.
2. Navigate to the root `/bootstrap` directory, then run `npm install`. npm will look at [package.json](package.json) and automatically install the necessary local dependencies listed there.

When completed, you'll be able to run the various Grunt commands provided from the command line.

**Unfamiliar with `npm`? Don't have node installed?** That's a-okay. npm stands for [node packaged modules](http://npmjs.org/) and is a way to manage development dependencies through node.js. [Download and install node.js](http://nodejs.org/download/) before proceeding.

### Available Grunt commands

#### Build - `grunt`
Run `grunt` to run tests locally and compile the CSS and JavaScript into `/dist`. **Uses [recess](http://twitter.github.io/recess/) and [UglifyJS](http://lisperator.net/uglifyjs/).**

#### Only compile CSS and JavaScript - `grunt dist`
`grunt dist` creates the `/dist` directory with compiled files. **Uses [recess](http://twitter.github.io/recess/) and [UglifyJS](http://lisperator.net/uglifyjs/).**

#### Tests - `grunt test`
Runs [JSHint](http://jshint.com) and [QUnit](http://qunitjs.com/) tests headlessly in [PhantomJS](http://phantomjs.org/) (used for CI).

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

For more information on SemVer, please visit <http://semver.org/>.



## Author

**Hamed Ramezanian**

+ [http://twitter.com/iceage2098](http://twitter.com/iceage2098)
+ [http://github.com/iCEAGE](http://github.com/iCEAGE)



## Copyright and license

[the Apache 2.0 license](LICENSE).
