## kata-js-vowel-count
Kata JS : compter les voyelles dans une chaîne : https://www.codewars.com/kata/54ff3102c1bad923760001f3

## Instructions
Return the number (count) of vowels in the given string.  
We will consider `a`, `e`, `i`, `o`, `u` as vowels for this Kata (but not `y`).  

The input string will only consist of lower case letters and/or spaces.  
FUNDAMENTALS STRINGS UTILITIES

## Mon code
```js
function getCount(str) {
  // Regex comptant les voyelles à l'exception du "y"
  var tabVoyelle = str.match(/[aeiou]/gi);
  return tabVoyelle === null ? 0 : tabVoyelle.length;
}
```

## Solution de la communauté
```js
function getCount(str) {
  return (str.match(/[aeiou]/ig)||[]).length;
}
```

## Docs
- String match : https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Global_Objects/String/match
- null : https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Global_Objects/null
