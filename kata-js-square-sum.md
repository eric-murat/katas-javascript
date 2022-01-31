Kata JS : Square(n) Sum - https://www.codewars.com/kata/515e271a311df0350d00000f

## Instructions
Complete the square sum function so that it squares each number passed into it and then sums the results together.  
For example, for `[1, 2, 2]` it should return `9` because `1^2 + 2^2 + 2^2 = 9`.  
✒️ FUNDAMENTALS, ARITHMETIC, MATHEMATICS, ALGORITHMS, NUMBERS, ARRAYS, LISTS, DATA STRUCTURES

## Mon code
```js
function squareSum(numbers){
  return numbers.map(item => item * item).reduce((prev,curr) => prev + curr,0);
}
```

## Code de la communauté
```js
function squareSum(numbers){
  return numbers.reduce(function(sum, n){
    return (n*n) + sum;
  }, 0)
}
```

## Docs
- Array map : https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/map
- Array reduce : https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/Reduce
