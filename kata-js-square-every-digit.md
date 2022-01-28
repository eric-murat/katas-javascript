# kata-js-square-every-digit
Kata JS : Square Every Digit https://www.codewars.com/kata/546e2562b03326a88e000020

## Instructions
Welcome. In this kata, you are asked to square every digit of a number and concatenate them.  
For example, if we run 9119 through the function, 811181 will come out, because 92 is 81 and 12 is 1.  
Note: The function accepts an integer and returns an integer  
FUNDAMENTALSMATHEMATICSALGORITHMSNUMBERS

## Mon code
```js
function squareDigits(num){
  var result = "";
  // Pour chaque digit, on ajoute "digit * digit" au résultat
  num.toString().split('').forEach(element => result = result + (element * element));
  return Number(result);
}
```
# Solution communauté
```js
function squareDigits(num){
  return Number(('' + num).split('').map(function (val) { return val * val;}).join(''));
}
```

# Docs
- Array forEach : https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/forEach
- Number : https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Global_Objects/Number
- String split : https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/split
