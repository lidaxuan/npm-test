# safeGet

``npm i @lijixuan/safe-get``

```js

const safeGet = require("@lijixuan/safe-get");

const data = {
  "a": {
    "b": {
      "c": [
        null,
        {
          "d": "hello world"
        }
      ]
    }
  }
};

const value = safeGet(data, "a.b.c[1].d");
// value = "hello world"
```