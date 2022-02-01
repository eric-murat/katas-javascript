Kata JS : Equal Sides Of An Array

## Instructions

## Mon code
```js
function findEvenIndex(arr) {
  var sumA = 0;
  var sumB = 0;
  var indexOk = -1;
  for (var i=0; i < Math.floor(arr.length / 2); i++) {
    sumA = sumA + arr[i];
    sumB = sumB + arr[arr.length - i - 1];
    if (sumA == sumB) {
      indexOk = i+1;
    }
  }
  return indexOk;
}
```

## Code de la communauté
```js

```

## Docs
- for : https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/for
- Math floor : https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math/floor
