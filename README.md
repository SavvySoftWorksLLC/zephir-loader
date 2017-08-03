# zephir loader for webpack

This package will compile your zephir code.

Ex:

## Installation

<del>`npm install zephir-loader`</del>

## Usage

``` javascript
var fileContent = require("zephir-loader!./file.php");
// => run file.php with php and return it as some content (html for example)
```

It can also be used inside the webpack configuration file (webpack.js):


``` javascript
module.exports = {
  ...
  module: {
    loaders: [
      ...
      {
        test: /\.zep$/,
        loaders: [
          'zephir-loader'
        ]
      },
      ...
    ]
  },
  ...
}
```

[Documentation: Using loaders](http://webpack.github.io/docs/using-loaders.html)

## License

MIT (http://www.opensource.org/licenses/mit-license.php)
