# kata-js-regex-replace-vowels
Kata JS : remplacer les voyelles dans une chaîne https://www.codewars.com/kata/52fba66badcd10859f00097e

## Instructions
Trolls are attacking your comment section!  
A common way to deal with this situation is to remove all of the vowels from the trolls' comments, neutralizing the threat.  
Your task is to write a function that takes a string and return a new string with all vowels removed.  
For example, the string "This website is for losers LOL!" would become "Ths wbst s fr lsrs LL!".  
*<ins>Note</ins>: for this kata y isn't considered a vowel.*  
✒️FUNDAMENTALS STRINGS REGULAR EXPRESSIONS DECLARATIVE PROGRAMMING ADVANCED LANGUAGE FEATURES

## Mon code
```js
function disemvowel(str) {
  return str.replace(/[aeiou]/ig, word => '');
}
```

## Code de la communauté
```js
function disemvowel(str) {
  return str.replace(/[aeiou]/ig, '');
}
```

## Docs
- String replace : https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Global_Objects/String/replace

