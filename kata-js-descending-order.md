Kata JS : Descending Order : https://www.codewars.com/kata/5467e4d82edf8bbf40000155/train/javascript

## Instructions
Your task is to make a function that can take any non-negative integer as an argument and return it with its digits in descending order. Essentially, rearrange the digits to create the highest possible number.

Examples:
```
Input: 42145 Output: 54421
Input: 145263 Output: 654321
Input: 123456789 Output: 987654321
```
✒️ FUNDAMENTALS

## Mon code
```js
function descendingOrder(n){
  var chars = (''+n).split('');
  chars.sort(function(a, b) {
    return b - a;
  });
  return parseInt(chars.join(''));
}
```

## Code de la communauté
```js
function descendingOrder(n){
  return parseInt(String(n).split('').sort().reverse().join(''))
}
```

## Docs
- Arrays.sort : https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Global_Objects/Array/sort
