# grunt-cssjanus

> Grunt plugin to convert CSS stylesheets between left-to-right and right-to-left

## Getting Started
This plugin requires Grunt `~0.4.1`

If you haven't used [Grunt](http://gruntjs.com/) before, be sure to check out the [Getting Started](http://gruntjs.com/getting-started) guide, as it explains how to create a [Gruntfile](http://gruntjs.com/sample-gruntfile) as well as install and use Grunt plugins. Once you're familiar with that process, you may install this plugin with this command:

```shell
npm install grunt-cssjanus --save-dev
```

Once the plugin has been installed, it may be enabled inside your Gruntfile with this line of JavaScript:

```js
grunt.loadNpmTasks('grunt-cssjanus');
```

## The "cssjanus" task

### Overview
In your project's Gruntfile, add a section named `cssjanus` to the data object passed into `grunt.initConfig()`.

```js
grunt.initConfig({
  cssjanus: {
    options: {
      // Task-specific options go here.
    },
    your_target: {
      // Target-specific file lists and/or options go here.
    },
  },
})
```

### Options

#### options.swapLtrRtlInUrl
Type: `Boolean`
Default value: `false`

Wheter to replce 'ltr' with 'rtl' and vice versa in urls.

#### options.swapLeftRightInUrl
Type: `Boolean`
Default value: `false`

Wheter to replce 'left' with 'right' and vice versa in urls.


### Usage Examples

#### Default Options
In this example, the default options are used to do something with whatever. So if the `testing` file has the content `Testing` and the `123` file had the content `1 2 3`, the generated result would be `Testing, 1 2 3.`

```js
grunt.initConfig({
  cssjanus: {
    options: {},
    files: {
      'dest/default_options': ['src/testing', 'src/123'],
    },
  },
})
```

## Release History
_(Nothing yet)_
