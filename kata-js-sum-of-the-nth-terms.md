Kata JS : Sum of the Nth terms of a series https://www.codewars.com/kata/555eded1ad94b00403000071

## Intructions
**Task:**  
Your task is to write a function which returns the sum of following series upto nth term(parameter).
```
Series: 1 + 1/4 + 1/7 + 1/10 + 1/13 + 1/16 +...
```
**Rules:**  
- You need to round the answer to 2 decimal places and return it as String.
- If the given value is 0 then it should return 0.00
- You will only be given Natural Numbers as arguments.

**Examples:(Input --> Output)**  
```
1 --> 1 --> "1.00"
2 --> 1 + 1/4 --> "1.25"
5 --> 1 + 1/4 + 1/7 + 1/10 + 1/13 --> "1.57"
```
✒️ FUNDAMENTALS, LOOPS, CONTROL FLOW, BASIC LANGUAGE FEATURES, ARITHMETIC, MATHEMATICS, ALGORITHMS, NUMBERS, SEQUENCES, ARRAYS

## Mon code
```js
function SeriesSum(n) {
  if (n === 0) return "0.00";
  var res = 0;
  for (var i = 0; i < n; i++) {
    res = res + 1 / (1 + i*3);
  }
  return res.toFixed(2);
}
```

## Code de la communauté
```js
function SeriesSum(n) {
  for (var s = 0, i = 0; i < n; i++) {
    s += 1 / (1 + i * 3)
  }
  
  return s.toFixed(2)
}
```

## Docs
- Number toFixed : https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Global_Objects/Number/toFixed
