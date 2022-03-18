Kata JS : Sum of Numbers https://www.codewars.com/kata/55f2b110f61eb01779000053

## Instructions
Given two integers a and b, which can be positive or negative, find the sum of all the integers between and including them and return it. If the two numbers are equal return a or b.

Note: a and b are not ordered!

Examples (a, b) --> output (explanation)
```
(1, 0) --> 1 (1 + 0 = 1)
(1, 2) --> 3 (1 + 2 = 3)
(0, 1) --> 1 (0 + 1 = 1)
(1, 1) --> 1 (1 since both are same)
(-1, 0) --> -1 (-1 + 0 = -1)
(-1, 2) --> 2 (-1 + 0 + 1 + 2 = 2)
```
✒️ FUNDAMENTALS, ALGORITHMS

## Mon code
```js
function getSum( a,b ) {
  var tab = [a,b].sort((a,b)=>a-b);
  var res = 0;
  for (var i = tab[0]; i <= tab[1]; i++) {
    res = res + i;
  }
  return res;
}
```

## Code de la communauté
```js
const GetSum = (a, b) => {
  let min = Math.min(a, b),
      max = Math.max(a, b);
  return (max - min + 1) * (min + max) / 2;
}
```

## Docs
- Array sort : https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/sort

