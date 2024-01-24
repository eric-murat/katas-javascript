Kata JS : ROT13 https://www.codewars.com/kata/52223df9e8f98c7aa7000062

✒️ FUNDAMENTALS, STRINGS, BASIC LANGUAGE FEATURES

## Mon code
```js
function rot13(str) {
  let result = "";
  let charCode;
  for (let i=0; i < str.length; i++) {
    charCode = str.charCodeAt(i);
    // Caractères majuscules
    if (charCode >= 65 && charCode <= 90) {
      charCode = 65 + (charCode - 65 + 13) % 26;
    } else if (charCode >= 97 && charCode <= 122) {
    // Caractères minuscules
      charCode = 97 + (charCode - 97 + 13) % 26;
    }
    result = result + String.fromCharCode(charCode);
  }
  return result;
```
## Code de la communauté
```js
function rot13(str) {
  return str.replace(/[a-z]/ig, function(x){
    return String.fromCharCode(x.charCodeAt(0) + (x.toLowerCase() <= 'm' ? 13: -13));
  });
}
```

## Docs
- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/fromCharCode
- https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/charCodeAt
- Table ASCII : https://www.techonthenet.com/ascii/chart.php
