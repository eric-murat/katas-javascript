# kata-js-find_unique
Kata JS : find the unique number : https://www.codewars.com/kata/585d7d5adb20cf33cb000235

## Instructions
There is an array with some numbers. All numbers are equal except for one. Try to find it!
```js
findUniq([ 1, 1, 1, 2, 1, 1 ]) === 2
findUniq([ 0, 0, 0.55, 0, 0 ]) === 0.55
```
It’s guaranteed that array contains at least 3 numbers.  
The tests contain some very huge arrays, so think about performance.  
FUNDAMENTALSALGORITHMSNUMBERSARRAYS

## Mon code
```js
function findUniq(arr) {
  arr.sort();
  var i1 = arr[0];
  var i2 = arr[1];
  var i3 = arr[2];
  // Cas particulier 1
  if (i1 != i2) return i1;
  // Cas particulier 2
  if ((arr.length == 3) && (i2 != i3)) return i3;
  for (var i = 3; i < arr.length; i++) {
    // Cas du dernier élément
    if ((i == arr.length - 1) && (arr[i] != i3)) return arr[i];
    // Cas élément intermédiaire
    if ((i2 != i3) && (arr[i] != i3)) return i3;
    // sinon, on décale
    i1 = arr[i - 2];
    i2 = arr[i - 1];
    i3 = arr[i];
  }
  return null;
}
```

## Solution de la communauté
```js
function findUniq(arr) {
  return arr.find(n => arr.indexOf(n) === arr.lastIndexOf(n));
}
```

## Docs
- Boucle for : https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Statements/for
- Array sort : https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Global_Objects/Array/sort
