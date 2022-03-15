Kata JS : Build tower : 

## Instructions

## Mon code
```js
function towerBuilder(nFloors) {
  var res = [];
  for (var i=0; i < nFloors; i++) {
    res.push(" ".repeat(nFloors - (i+1)) + "*".repeat((i+1)*2 - 1) + " ".repeat(nFloors - (i+1)));
  }
  return res;
}
```
## Code de la communauté
```js
function towerBuilder(nFloors) {
  var res = [];
  for (var i=0; i < nFloors; i++) {
    res.push(" ".repeat(nFloors - (i+1)) + "*".repeat((i+1)*2 - 1) + " ".repeat(nFloors - (i+1)));
  }
  return res;
}
```

## Docs
- String repeat : https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/repeat
