Kata JS : Are they the same ?

## Instructions

## Mon code
```js
function comp(array1, array2){
  if (Array.isArray(array1) && Array.isArray(array2)) {
    array1.sort((a, b) => a - b);
    array2.sort((a, b) => a - b);
    for (var i=0; i < array1.length; i++) {
      if (array1[i] * array1[i] != array2[i]) {
        return false;
      }
    }
    return true;
  } else {
    if (Array.isArray(array1)) {
        return array2 !== null;
    }
    if (Array.isArray(array2)) {
        return array1 !== null;
    }
  }
}
```

## Code de la communauté
```js
function comp(array1, array2) {
  if(array1 == null || array2 == null) return false;
  array1.sort((a, b) => a - b); array2.sort((a, b) => a - b);
  return array1.map(v => v * v).every((v, i) => v == array2[i]);
}
```

## Docs
- null : https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Global_Objects/null
- Array sort : https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/sort
