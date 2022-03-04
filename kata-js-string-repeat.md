Kata JS : String repeat

## Instructions

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
