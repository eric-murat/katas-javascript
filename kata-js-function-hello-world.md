# kata-js-find_unique
Kata JS : function hello world : https://www.codewars.com/kata/585d7d5adb20cf33cb000235

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
function greet() {
  return "hello world!";
}```

## Solution de la communauté
```js
function findUniq(arr) {
  return arr.find(n => arr.indexOf(n) === arr.lastIndexOf(n));
}
```

## Docs
- Boucle for : https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Statements/for
- Array sort : https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Global_Objects/Array/sort
