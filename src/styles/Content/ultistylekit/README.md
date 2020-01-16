# [UltiStyleKit](http://devgit:7990/projects/USK/repos/ultistylekit/browse)

UltiStyleKit is a thin set of overrides on top of Bootstrap 3. It takes the [SMACSS](https://smacss.com/) modular approach at providing a set of reusable components that can be used to achieve the look and feel of an UltiPro v14/16 application.

Access the current StyleGuide here: http://ux.ultimatesoftware.com/styleguide/#/

## Getting Started

### Bower

UltiStyleKit is available as a bower package. It is not available in the public
bower repository though, so you must specify the full URL to this Stash repo.
You can install it via

```
bower install --save http://devgit.dev.us.corp:7990/scm/usk/ultistylekit.git
```

If your team is using LESS, update your compilation settings to include your
bower components path in the list of `--include-paths`. (See instructions for
[Grunt](https://github.com/gruntjs/grunt-contrib-less#paths),
[Gulp](https://github.com/plus3network/gulp-less#options), or
[lessc](http://lesscss.org/usage/#command-line-usage-options).) If your bower
components path is non-standard, you will need to modify your LESS build to
revise the root path for font and image assets. See [UltiStyleKit's
Gruntfile.js](http://devgit:7990/projects/USK/repos/ultistylekit/browse/Gruntfile.js#25)
for an example.

If you are not using LESS, you may instead choose to use the pre-compiled
`dist` directory. Bootstrap and Font-Awesome are embedded directly into
`ultistylekit.css`, while jQuery and Bootstrap's JS are embedded in
`ultistylekit.js`. Additionally, all image and font asset paths are rewritten
to reference the structure laid out in `dist`. Thus, ensure all of the contents
of the `dist` directory are available in your production build environment.

### Pre-compiled ZIP

If your project is not using Bower for front-end dependency management, you can
use the pre-compiled zip available in this repo. You can also download the zip
directly from http://ux.ultimatesoftware.com/ultistylekit/ultistylekit.zip.

## Updated Visual Design

Once you have the UltiStyleKit package installed, you'll find two versions of
the CSS/LESS available. `ultistylekit.legacy.css` is the original v14 UltiPro
styling. Use this version if you need a low-impact change when upgrading to
UltiStyleKit 2.0. `ultistylekit.css` is the new visual design that will roll
out later in 2015. If you're starting a new project, use this version instead
of `legacy`.

## Getting the Source Code

1. Install [NodeJS](http://nodejs.org/)

2. Install [Grunt](http://gruntjs.com/getting-started): `npm install -g grunt-cli`

3. Install [Bower](http://bower.io/): `npm install -g bower`

4. Clone: `git clone http://devgit:7990/scm/usk/ultistylekit.git && cd ultistylekit`

5. Install: `npm install` && `bower install`

6. Build: `grunt build`

## Versioning

UltiStyleKit follows [Semantic Versioning](http://semver.org) as of 2.0.0. See
the [CHANGELOG](CHANGELOG.md) for release notes.

With this change, UltiStyleKit 1.0.7 will no longer be supported but can be
downloaded from the **v1.0.7** tag as follows:

```
git clone --branch v1.0.7 http://devgit:7990/scm/usk/ultistylekit.git
```

## Maintainers

* [Gunther Taborga](<gunther_taborga@ultimate_software.com>) (Author)
* [Jeff Tucker](<jeff_tucker@ultimatesoftware.com>) (Maintainer)
