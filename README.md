# Autodraw API wrapper

## Installation

```
npm install --save autodraw
```

## Usage

```js
const autodraw = require('autodraw')

const shape1 = [
  {
    x: 10,
    y: 5
  },
  {
    x: 40,
    y: 10
  }
]

const shapes = [
  shape1
]

autodraw(shapes).then(results => {
  /* array of recognized objects:
   * [{
   *    name,
   *    confidence (closer to 0 == more confident),
   *    url (url to a svg representing the object),
   *    url_variant_1,
   *    url_variant_2
   * }]
   */
})
```

## Licence

MIT

