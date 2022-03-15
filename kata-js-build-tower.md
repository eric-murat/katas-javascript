Kata JS : Build tower : https://www.codewars.com/kata/576757b1df89ecf5bd00073b

## Instructions
Build Tower
Build a pyramid-shaped tower given a positive integer number of floors. A tower block is represented with "*" character.

For example, a tower with 3 floors looks like this:
```
[
  "  *  ",
  " *** ", 
  "*****"
]
```
And a tower with 6 floors looks like this:
```
[
  "     *     ", 
  "    ***    ", 
  "   *****   ", 
  "  *******  ", 
  " ********* ", 
  "***********"
]
```
✒️ FUNDAMENTALS, STRINGS, BASIC LANGUAGE FEATURES

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
function towerBuilder(n) {
  return [...Array(n)].map((_,i)=>" ".repeat(n-1-i)+"*".repeat(i*2+1)+" ".repeat(n-1-i))
}
```

## Docs
- String repeat : https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/repeat
