# Critical-Starter

[ ![Codeship Status for Bigalan09/critical-starter](https://app.codeship.com/projects/1b742ea0-a2c3-0135-436c-7a11b80692af/status?branch=master)](https://app.codeship.com/projects/254761)

A basic HTML5, Bootstrap 4, JQuery and Font-Awesome starter project using Critical to improve pagespeed insight score.

Generate and inline critical-path CSS using [Critical](http://github.com/addyosmani/critical).
Thanks to [Critical Path Demo](https://github.com/addyosmani/critical-path-css-demo)

## Installation

```sh
$ cd critical-starter
$ yarn && bower install
```

## Generating and inlining critical-path CSS

**Note: There are two build commands available. This allows you to compare the difference
between the output of a normal build and the output with critical-path CSS.**

The default (minify, concat) build for the project can be run with:

```sh
$ gulp
```

The complete (critical-path) build can be run with:

```sh
$ gulp critical
```

This performs the normal build, then generates and inlines critical-path CSS for the page. It automatically async loads in the site-wide styles using [loadCSS](https://github.com/filamentgroup/loadCSS/) as part of the workflow offered by the module.
