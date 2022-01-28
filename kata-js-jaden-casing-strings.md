# kata-js-jaden-casing-strings
Kata JS : Jaden Casing Strings https://www.codewars.com/kata/5390bac347d09b7da40006f6

## Instructions
Jaden Smith, the son of Will Smith, is the star of films such as The Karate Kid (2010) and After Earth (2013). Jaden is also known for some of his philosophy that he delivers via Twitter. When writing on Twitter, he is known for almost always capitalizing every word. For simplicity, you'll have to capitalize each word, check out how contractions are expected to be in the example below.

Your task is to convert strings to how they would be written by Jaden Smith. The strings are actual quotes from Jaden Smith, but they are not capitalized in the same way he originally typed them.

<ins>Exemple:</ins>
```
Not Jaden-Cased: "How can mirrors be real if our eyes aren't real"
Jaden-Cased:     "How Can Mirrors Be Real If Our Eyes Aren't Real"
```
✒️ FUNDAMENTALS STRINGS ARRAYS

## Mon code
```js
String.prototype.toJadenCase = function () {
  //return this.replace(/([^ \t]+)/g, function(word) { return word[0].toUpperCase() + word.slice(1); });
  return this.replace(/([^ \t]+)/g, word => word[0].toUpperCase() + word.slice(1));

  // A noter pour info : cette formule bug sur "[..] aren't real" --> "Aren\'T Real" :
  //return this.replace(/\w+/g, word => word[0].toUpperCase() + word.slice(1));
};
```

## Code de la communauté
```js
String.prototype.toJadenCase = function () {
  return this.split(' ').
    map(w => w[0].toUpperCase() + w.slice(1)).join(' ');
};
```

## Docs
- String replace regex : https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/replace
- Expressions rationnelles : https://developer.mozilla.org/fr/docs/Web/JavaScript/Guide/Regular_Expressions
- String .split : https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/split
- Array .join : https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/join
- Array .map : https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/map
