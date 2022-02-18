Kata JS : Highest scoring word 

## Instructions

## Mon code
```js
function high(x){
  return x.split(' ').reduce((previousValue, currentValue) => {
     if (currentValue.split('').reduce((a,b) => {
         return a + b.charCodeAt(0)-96;  // car "A" charCode = 97
       },0) > previousValue.split('').reduce((c, d) => {
         return c + d.charCodeAt(0)-96;  // car "A" charCode = 97
       },0)) {
       return currentValue;
     } else {
       return previousValue;
     }
  });
}
```

## Code de la communauté
```js
```

## Docs
- String split : https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/split
- Array reduce : https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/Reduce
- String charCodeAt : https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Global_Objects/String/charCodeAt

