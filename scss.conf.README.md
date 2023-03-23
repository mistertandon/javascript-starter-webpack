#### SCSS configuration
<br/>

`$ npm install --save-dev sass sass-loader style-loader css-loader`

<br/>
> Update your webpack.config.js file to use SCSS. Here's an example:

```javascript
const path = require('path');

module.exports = {
  ...,
  module: {
    rules: [
      {
        test: /\.scss$/,
        use: [
          'style-loader',
          'css-loader',
          'sass-loader',
        ],
      },
    ],
  },
};

```

> Update your package.json file to run build cmd:

```json
{
"scripts": {
 "build": "webpack"
}}
```

`$ npm run build`
