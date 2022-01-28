# kata-js-break-camelcase
Kata JS : Break camelCase https://www.codewars.com/kata/5208f99aee097e6552000148


## Instructions
Complete the solution so that the function will break up camel casing, using a space between words.  
Example
```
"camelCasing"  =>  "camel Casing"
"identifier"   =>  "identifier"
""             =>  ""
```
✒️FUNDAMENTALS STRINGS FORMATTING ALGORITHMS

## Mon code :
```js
function solution(string) {
  // Remplacement des lettres majuscule par ' ' + lettre
  return string.replace(/[A-Z]/g, function(match, offset, string) {
    return (offset > 0 ? ' ' : '') + match;
  });
}
```
## Meilleure solution de la communauté :
```js
function solution(string) {
  return(string.replace(/([A-Z])/g, ' $1'));
}
```

## Docs :
- String.replace : https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/replace
