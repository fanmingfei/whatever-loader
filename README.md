# whatever-loader
Load whatever u wanna loader with webpack.


## Install
```bash
npm install --save-dev whatever-loader
```

## Usage

The `whatever-loader` can loader whatever file to your program, you will get the file content.

**file.js**

```js
import tpl from 'file.tpl';

import json from 'json-file.json';

import conf from 'config.conf';
```


**webpack.config.js**

```js
module.exports = {
  module: {
    rules: [
      {
        test: /\.tpl$/,
        use: [ 'whatever-loader' ]
      },
      {
        test: /\.json$/,
        use: [ 'whatever-loader' ]
      },
      {
        test: /\.conf$/,
        use: [ 'whatever-loader' ]
      }
    ]
  }
}
```