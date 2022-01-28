# kata-js-convert-number-reversed-array
Kata JS : Convert number to reversed array of digits https://www.codewars.com/kata/5583090cbe83f4fd8c000051

## Instructions
Convert number to reversed array of digits  
Given a random non-negative number, you have to return the digits of this number within an array in reverse order.  
Example:
```
348597 => [7,9,5,8,4,3]
0 => [0]
```
✒️ FUNDAMENTALS NUMBERS ARRAYS

## Mon code
```js
function digitize(n) {
  return (""+n).split('').map(function (val) {return parseInt(val);}).reverse();
}
```

## Code de la communauté
```js
function digitize(n) {
  return String(n).split('').map(Number).reverse()
}
```

## Docs
- String split : https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Global_Objects/String/split
- Array reverse : https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Global_Objects/Array/reverse
- parseInt : https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Global_Objects/parseInt
- Array map : https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Global_Objects/Array/map
