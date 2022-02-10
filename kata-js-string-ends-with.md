Kata JS : String ends with https://www.codewars.com/kata/51f2d1cafc9c0f745c00037d

## Instructions
Complete the solution so that it returns true if the first argument(string) passed in ends with the 2nd argument (also a string).

Examples:
```
solution('abc', 'bc') // returns true
solution('abc', 'd') // returns false
```
✒️ FUNDAMENTALS, STRINGS

## Mon code
```js
function solution(str, ending){
  return ending.length <= 0 ? true : ending == str.slice(-1 * ending.length);
}
```

## Code de la communauté
```js
function solution(str, ending){
  return str.endsWith(ending);
}
```

## Docs
- Array slice : https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/slice
