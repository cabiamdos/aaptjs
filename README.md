# aaptjs

A node wraper for aapt

# Install

With [npm](https://npmjs.org/package/@cabiam/aaptjs) do:

```
npm install @cabiam/aaptjs --save
```

## Example
Using a callback:
```js
const aaptjs = require('@cabiam/aaptjs');

aaptjs.list('/path/to/your/ExampleApp.apk', (err, data) => {
  if (err) {
    // something went wrong 
  } else {
    console.log(data);
  }
});
```

Using a promise:

```js
const aaptjs = require('aaptjs');

aaptjs.list('/path/to/your/ExampleApp.apk')
  .then (data => {
    console.log(data)
  })
  .catch (err) {
    // something went wrong 
  }

```

## Acknowledment

https://github.com/vldmkr/node-aapt
https://github.com/shenzhim/aaptjs
