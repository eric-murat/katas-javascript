# kata-js-isisogram
Kata JS - Isograms : https://www.codewars.com/kata/54ba84be607a92aa900000f1

# Instructions
An isogram is a word that has no repeating letters, consecutive or non-consecutive. Implement a function that determines whether a string that contains only letters is an isogram. Assume the empty string is an isogram. Ignore letter case.

Example: (Input --> Output)
```
"Dermatoglyphics" --> true
"aba" --> false
"moOse" --> false (ignore letter case)
```
✒️FUNDAMENTALS, STRINGS

# Mon code
```js
function isIsogram(str){
  // 1. On transforme tous les caractères en minuscules
  str = str.toLowerCase();
  // 2. Pour chaque caractère, on vérifie que son .indexOf correspond à l'index en cours
  return str.split('').every((c, i) => str.indexOf(c) == i);
}
```

# Source correction
https://stackoverflow.com/questions/50134662/check-that-a-word-is-an-isogram-with-pure-javascript/50134936
```
let isIsogram = (str) => str.split("").every((c, i) => str.indexOf(c) == i);
                            
console.log(isIsogram("thomas"));   /* no repeating letter */
console.log(isIsogram("moses"));    /* s repeat 2 times */
console.log(isIsogram("hello"));    /* l repeat 2 times */
console.log(isIsogram("world"));    /* no repeating letter */
console.log(isIsogram("a b c"));    /* space character repeat 2 times */
```
# Docs
- String split : https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/split
- Array every : https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/every
```
[12, 5, 8, 130, 44].every(elem => elem >= 10); // false
[12, 54, 18, 130, 44].every(elem => elem >= 10); // true
[{a:1, b:2}, {a:1, b:3}].every(elem => elem.a === 1); // true
[{a:2, b:2}, {a:1, b:3}].every(elem => elem.a === 1); // false
```
- Truthy value : https://developer.mozilla.org/en-US/docs/Glossary/Truthy
- Fonction fléchée => : https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Functions/Arrow_functions
```js
var a = [
  "We're up all night 'til the sun",
  "We're up all night to get some",
  "We're up all night for good fun",
  "We're up all night to get lucky"
];

// Sans la syntaxe des fonctions fléchées
var a2 = a.map(function (s) { return s.length });
// [31, 30, 31, 31]

// Avec, on a quelque chose de plus concis
var a3 = a.map( s => s.length);
// [31, 30, 31, 31]
```
- Arrow function : https://www.w3schools.com/js/js_arrow_function.asp
