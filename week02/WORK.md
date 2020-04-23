# 作业





- 写一个正则表达式 匹配所有 Number 直接量
```js
/^[+-]?((\d+|\d*\.\d*)(e[+-]?\d+|)|0b[01]+|0o[0-7]+|0x[\dabcdef]+)$/i
```
https://codesandbox.io/s/number-regexp-fbr6o


- 写一个 UTF-8 Encoding 的函数
```js
function encodeUtf8(text) {
  const code = encodeURIComponent(text);
  const bytes = [];
  for (var i = 0; i < code.length; i++) {
    const c = code.charAt(i);
    if (c === "%") {
      const hex = code.charAt(i + 1) + code.charAt(i + 2);
      const hexVal = parseInt(hex, 16);
      bytes.push(hexVal);
      i += 2;
    } else {
      bytes.push(c.charCodeAt(0));
    }
  }
  console.log(bytes);
  return bytes;
}

```
https://codesandbox.io/s/encodeutf8-decodeutf8-7weko


- 写一个正则表达式，匹配所有的字符串直接量，单引号和双引号
```js
/^('(\\'|[^ '\n\r\u2028\u2029]|\s)*'|"(\\"|[^ "\n\r\u2028\u2029]|\s)*")$/i
```
https://codesandbox.io/s/string-regexp-g5qpk
