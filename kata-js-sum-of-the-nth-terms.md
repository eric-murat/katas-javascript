Kata JS : Sum of the Nth terms of a series 

## Intructions

## Mon code
```js
```

## Code de la communauté
```js
function SeriesSum(n) {
  for (var s = 0, i = 0; i < n; i++) {
    s += 1 / (1 + i * 3)
  }
  
  return s.toFixed(2)
}
```

## Docs
- Number toFixed : https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Global_Objects/Number/toFixed
