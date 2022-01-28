# kata-js-sum-lowest-int
Kata JS : Sum of two lowest positive integers https://www.codewars.com/kata/558fc85d8fd1938afb000014

## Instructions
Create a function that returns the sum of the two lowest positive numbers given an array of minimum 4 positive integers.  
No floats or non-positive integers will be passed.  
For example, when an array is passed like [19, 5, 42, 2, 77], the output should be 7.  
```
[10, 343445353, 3453445, 3453545353453] should return 3453455.
```
✒️ FUNDAMENTALS ARRAYS

## Mon code
```js
function sumTwoSmallestNumbers(numbers) {  
  return numbers.sort((a,b)=>a-b).slice(0,2).reduce((prev,curr)=>prev+curr);
}
```

## Code de la communauté
```js
function sumTwoSmallestNumbers(numbers){  
  numbers = numbers.sort(function(a, b){return a - b; });
  return numbers[0] + numbers[1];
};
```

## Docs
- Array sort https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/sort  
  - Tri par défaut : basé sur les caractères
    ```js
    return [3, 87, 45, 12, 7].sort();
    // Result = [ 12, 3, 45, 7, 87 ]
    ```
  - Tri par ordre croissant numérique
    ```js
    return [3, 87, 45, 12, 7].sort((a,b)=>a-b);
    // Result = [ 3, 7, 12, 45, 87 ]
    ```
  - Tri par ordre décroissant numérique
    ```js
    return [3, 87, 45, 12, 7].sort((a,b)=>b-a);
    // Result = [ 87, 45, 12, 7, 3 ]
    ```

- Array slice : https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/slice
```js
return [3, 87, 45, 12, 7].slice(0,1);
// Result = [ 3 ]

return [3, 87, 45, 12, 7].slice(2,5);  // 5 index hors limite mais bon :)
// Result = [ 45, 12, 7 ]
```

- Array reduce : https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/Reduce
```js
// Array sum
return [3, 2, 1, 4].reduce((prev,curr)=prev+curr);
// Result = 10
```
