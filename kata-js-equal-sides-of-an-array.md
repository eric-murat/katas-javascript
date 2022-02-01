Kata JS : Equal Sides Of An Array

## Instructions

## Mon code
```js
function findEvenIndex(arr) {
  if (arr.length == 0) return -1;
  for (var i=0; i < arr.length; i++) {
    if (arr.slice(0,i).reduce((a,b)=>a+b,0) == arr.slice(i+1).reduce((a,b)=>a+b,0)) {
      return i;
    }
  }
  return -1;
}
```

## Code de la communauté
```js

```

## Docs
- Array slice : https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/slice
- Array reduce : https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Global_Objects/Array/Reduce
