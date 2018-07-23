# mini-base64

## 安装
```
$ npm install mini-base64 --save
```

## 使用

```js
const { arrayBufferToBase64, base64ToArrayBuffer } = require('mini-base64');

const base64 = 'QUJDREVGR0hJSktMTU5PUFFSU1RVVldYWVphYmNkZWZnaGlqa2xtbm9wcXJzdHV2d3h5ejAxMjM0NTY3ODk=';
console.log(arrayBufferToBase64(base64ToArrayBuffer(base64)) === base64); // true

// 将 ArrayBuffer 数据转成 Base64 字符串
const arrayBuffer = new Uint8Array([11, 22, 33])
const base64 = arrayBufferToBase64(arrayBuffer)

// 将 Base64 字符串转成 ArrayBuffer 数据
const base64 = 'CxYh'
const arrayBuffer = base64ToArrayBuffer(base64)
```
