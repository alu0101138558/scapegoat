Scapegoat
=========

A minimal node module providing utility methods to `escape` and `unescape` HTML entities

See the associated blog post, ["Creating and publishing a node.js module."](https://quickleft.com/blog/creating-and-publishing-a-node-js-module/)

## Installation

```shell
  npm install @ull-esit-dsi-1617/scapegoat --save
```

## Usage

```js
  var scapegoat = require('@ull-esit-dsi-1617/scapegoat'),
      escape = scapegoat.escape,
      unescape = scapegoat.unescape;

  var html = '<h1>Hello World</h1>',
      escaped = escape(html),
      unescaped = unescape(escaped);

  console.log('html', html, 'escaped', escaped, 'unescaped', unescaped);
```

## Tests

```shell
   npm test
```

## API Documents

[See Documentation at https://ull-esit-dsi-1617.github.io/scapegoat/](https://ull-esit-dsi-1617.github.io/scapegoat/)

To generate the docs we use [documentation.js](http://documentation.js.org/):

```shell
   npm run doc
```

Install `$ npm install -g documentation`


## Contributing

In lieu of a formal styleguide, take care to maintain the existing coding style.
Add unit tests for any new or changed functionality. Lint and test your code.

## Release History

* 1.0.3 Scopes and API documentation
* 1.0.0 Refactor to avoid double unescape and to use npm scripts instead
  of makefile.  Also add link to associated blog post.
* 0.1.0 Initial release
