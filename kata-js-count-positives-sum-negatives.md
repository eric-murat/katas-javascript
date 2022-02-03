Kata JS : Count of positives / sum of negatives

## Instructions

## Mon code
```js
function countPositivesSumNegatives(input) {
    if (Array.isArray(input) && input.length > 0) {
      // Concat de "Count positive numbers" et "Sum negative numbers"
      return [].concat(input.filter((a) => a > 0).length).concat( input.filter((a) => a < 0).reduce((prev,curr) => prev + curr,0) );
    }
}
```

## Code de la communauté
```js
```

## Docs
- Array filter : https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/filter
- Array reduce : https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/Reduce
- Array concat : https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/concat
