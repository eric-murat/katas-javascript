Kata JS : String repeat https://www.codewars.com/kata/57a0e5c372292dd76d000d7e

## Instructions
Write a function called repeatStr which repeats the given string string exactly n times.
```
repeatStr(6, "I") // "IIIIII"
repeatStr(5, "Hello") // "HelloHelloHelloHelloHello"
```
✒️ FUNDAMENTALS

## Mon code
```js
function repeatStr (n, s) {
  for (var i=0, res=""; i < n; i++) {
    res = res + s;
  }
  return res;
}
```

## Code de la communauté
```js
function repeatStr (n, s) {
  return s.repeat(n);
}
```

## Docs
- String repeat : https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/repeat
