
## Mon code
```js
function squareSum(numbers){
  return numbers.map(item => item * item).reduce((prev,curr) => prev + curr,0);
}
```

## Code de la communauté
```js
function squareSum(numbers){
  return numbers.map(item => item * item).reduce((prev,curr) => prev + curr,0);
}
```

## Docs
- Array map : https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/map
- Array reduce : https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/Reduce
