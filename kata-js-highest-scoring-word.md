Kata JS : Highest scoring word https://www.codewars.com/kata/57eb8fcdf670e99d9b000272

## Instructions
Given a string of words, you need to find the highest scoring word.
Each letter of a word scores points according to its position in the alphabet: `a = 1, b = 2, c = 3` etc.
You need to return the highest scoring word as a string.
If two words score the same, return the word that appears earliest in the original string.
All letters will be lowercase and all inputs will be valid.

✒️FUNDAMENTAL, SSTRINGS, ARRAYS, NUMBERS

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
function high(s){
  let as = s.split(' ').map(s=>[...s].reduce((a,b)=>a+b.charCodeAt(0)-96,0));
  return s.split(' ')[as.indexOf(Math.max(...as))];
}
```

## Docs
- String split : https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/split
- Array reduce : https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/Reduce
- String charCodeAt : https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Global_Objects/String/charCodeAt

