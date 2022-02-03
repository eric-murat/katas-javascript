Kata JS : Count of positives / sum of negatives https://www.codewars.com/kata/576bb71bbbcf0951d5000044

## Instructions
Given an array of integers.  
Return an array, where the first element is the count of positives numbers and the second element is sum of negative numbers. 0 is neither positive nor negative.  
If the input array is empty or null, return an empty array.

Example
For input `[1, 2, 3, 4, 5, 6, 7, 8, 9, 10, -11, -12, -13, -14, -15]`, you should return `[10, -65]`.

✒️FUNDAMENTALS, ARRAYS, LISTS, DATA STRUCTURES, ARITHMETIC, MATHEMATICS, ALGORITHMS, NUMBERS

## Mon code
```js
function countPositivesSumNegatives(input) {
    if (Array.isArray(input) && input.length > 0) {
      // Concat de "Count positive numbers" et "Sum negative numbers"
      return [].concat(input.filter((a) => a > 0).length).concat( input.filter((a) => a < 0).reduce((prev,curr) => prev + curr,0) );
    } else {
      return [];
    }
}
```

## Code de la communauté
```js
function countPositivesSumNegatives(input) {
    return input && input.length ? [input.filter(p => p > 0).length, input.filter(n => n < 0).reduce((a, b) => a + b, 0)] : [];
}
```

## Docs
- Array filter : https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/filter
- Array reduce : https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/Reduce
- Array concat : https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/concat
- Array isArray : https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/isArray
