# Bower - Setup

> A few thoughts how to set up Bower - A package manager for the web.

- [Bower.js][bower-web]
- [Bower search][bower-search]
- [GitHub][bower-github]
- [npm][bower-npm]

## Install Bower:

Install `bower` globally and you'll have access to the bower command anywhere on your system.

- `$ npm install bower -g`

## Initialize Bower:

Creates `bower.json` project info file.

- `$ bower init`
 
bower.json
```javascript
{
  "name": "number-picker",
  "version": "0.0.1",
  "main": [
    "dist/js/numberPicker.js",
    "dist/css/numberPicker.css",
    "dist/img/numberPicker.png"
  ],
  "ignore": [
    "**/.*",
    "*.md",
    "demo",
    "lib",
    "node_modules",
    "src",
    ".bowerrc",
    ".gitattributes",
    ".gitignore",
    ".jshintrc",
    ".sublime-project",
    "Gruntfile.js",
    "package.json"
  ],
  "dependencies": {
    "jquery": ">= 1.9.0 < 2.0.0"
  },
  "devDependencies": {
    "bootstrap": "~3.1.1"
  }
}
```

## Install package:

Install a new package for instance `jquery` the latest version `1.x` and save it into dependencies.

- `$ bower install jquery#~1 --save`

## Uninstall package:

Uninstall a package for instance `jquery` from dependencies.

- `$ bower uninstall jquery --save`

## Check for updates:

Check for updates of all packages from dependencies.

- `$ bower list`

## Update all packages:

Update all packages from dependencies.

- `$ bower update`

## Install all packages:

Install all packages from dependencies.

- `$ bower install`

## Install private package:

Install a your private package.

- `$ bower install git@github.com:martinjezek/private-plugin.git --save`

[bower-web]: http://bower.io
[bower-search]:http://bower.io/search/
[bower-github]: https://github.com/bower/bower
[bower-npm]: https://www.npmjs.org/package/bower