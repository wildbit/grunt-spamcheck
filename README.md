# grunt-spamcheck

[![Built with Grunt](https://cdn.gruntjs.com/builtwith.png)](http://gruntjs.com/)
[![Build Status](https://travis-ci.org/derekrushforth/grunt-spamcheck.svg)](https://travis-ci.org/derekrushforth/grunt-spamcheck)

> Spam check your emails using [Postmark's](http://spamcheck.postmarkapp.com) API

## Getting Started

If you haven't used [Grunt](http://gruntjs.com/) before, be sure to check out the [Getting Started](http://gruntjs.com/getting-started) guide, as it explains how to create a [Gruntfile](http://gruntjs.com/sample-gruntfile) as well as install and use Grunt plugins. Once you're familiar with that process, you may install this plugin with this command:

```shell
npm install grunt-spamcheck --save-dev
```

After the plugin is installed, it can be enabled in your Gruntfile:

```js
grunt.loadNpmTasks('grunt-spamcheck');
```

## Spamcheck task
_Run this task with the `grunt spamcheck` command._

![grunt-spamcheck](grunt-spamcheck.png?raw=true)

## Options

### report
_Specifies whether you would like more detailed reporting._

Type: `String`

Default: `long`

Options: `short`, `long`


### hideGraph
_Specifies whether you want to hide the score graph._

Type: `Boolean`

Default: `false`


## Examples

```javascript
grunt.initConfig({
  spamcheck: {
    emails: {
      report: 'long',
      src: ['emails/template1.html', 'emails/template2.html', 'emails/template3.html']
    }
  }
});
```

## Tests
_Run this task with the `grunt test` command._