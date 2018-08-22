Panel component
===============

[![build status](https://img.shields.io/travis/magsdk/component-panel.svg?style=flat-square)](https://travis-ci.org/magsdk/component-panel)
[![npm version](https://img.shields.io/npm/v/mag-component-panel.svg?style=flat-square)](https://www.npmjs.com/package/mag-component-panel)
[![dependencies status](https://img.shields.io/david/magsdk/component-panel.svg?style=flat-square)](https://david-dm.org/magsdk/component-panel)
[![devDependencies status](https://img.shields.io/david/dev/magsdk/component-panel.svg?style=flat-square)](https://david-dm.org/magsdk/component-panel?type=dev)
[![Gitter](https://img.shields.io/badge/gitter-join%20chat-blue.svg?style=flat-square)](https://gitter.im/DarkPark/magsdk)


Panel is a component to build user interface, an instance of [Component](https://github.com/stbsdk/component) module. Use with [component-panel-set](https://github.com/magsdk/component-panel-set).



## Installation ##

```bash
npm install mag-component-panel
```


## Usage ##

Add the singleton to the scope:

```js
var Panel = require('mag-component-panel');
```

Create instance with custom config:
```js
var panel = new Panel({
        title: [
            {
                value: _('Menu'),
                className: 'name'
            }
        ],
        events: {
            focus: function () {}
        },
        children: [
            new LayoutList({
                cycle: true,
                data: [],
                fixedData: true,
                size: 6
            })
        ]
    });
```


## Development mode ##

> There is a global var `DEVELOP` which activates additional consistency checks and protection logic not available in release mode.


## Contribution ##

If you have any problems or suggestions please open an [issue](https://github.com/magsdk/component-panel/issues)
according to the contribution [rules](.github/contributing.md).


## License ##

`mag-component-panel` is released under the [MIT License](license.md).
