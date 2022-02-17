Kata JS : GarssHopper Summation https://www.codewars.com/kata/55d24f55d7dd296eb9000030

## Instructions
**Summation**
Write a program that finds the summation of every number from 1 to num. The number will always be a positive integer greater than 0.

For example:
```
summation(2) -> 3
1 + 2

summation(8) -> 36
1 + 2 + 3 + 4 + 5 + 6 + 7 + 8
```
✒️ FUNDAMENTALS, LOOPS, CONTROL FLOW, BASIC LANGUAGE FEATURES

## Mon code
```js
var summation = function (num) {
  for (var i=0, s=0; i <= num; i++) {
    s = s + i;
  }
  return s;
}
```

## Code de la communaauté
```js
var summation = function (num) {
  return num * (num+1) / 2;
}
```

## Docs
