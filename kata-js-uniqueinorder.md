Kata JS - Unique In Order : https://www.codewars.com/kata/54e6533c92449cc251001667

## Instructions
Implement the function unique_in_order which takes as argument a sequence and returns a list of items without any elements with the same value next to each other and preserving the original order of elements.

For example:
```
uniqueInOrder('AAAABBBCCDAABBB') == ['A', 'B', 'C', 'D', 'A', 'B']
uniqueInOrder('ABBCcAD')         == ['A', 'B', 'C', 'c', 'A', 'D']
uniqueInOrder([1,2,2,3,3])       == [1,2,3]
```
✒️FUNDAMENTALS, ADVANCED LANGUAGE FEATURES, ALGORITHMS

## Mon code
```js
var uniqueInOrder=function(iterable){
  //your code here - remember iterable can be a string or an array

  //const words = ['spray', 'limit', 'elite', 'exuberant', 'destruction', 'present'];
  //const result = words.filter(word => word.length > 6);
  //console.log(result);
  // expected output: Array ["exuberant", "destruction", "present"]  

  // Appending new words
  //words = ['spray', 'limit', 'exuberant', 'destruction', 'elite', 'present']
  //const appendedWords = words.filter( (word, index, arr) => {
  //  arr.push('new')
  //  return word.length < 6
  //})  
  //console.log(appendedWords);  

  return [...iterable].filter((elem, i, arr) => {
    arr.push('new')
    return elem != arr[i-1]
  });
}
```

## Docs
- Array filter : https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/filter
- Convertir une chaine en tableau avec [...iter] : https://www.delftstack.com/fr/howto/javascript/convert-string-to-array-javascript/
