Kata JS : Descending Order : https://www.codewars.com/kata/5467e4d82edf8bbf40000155/train/javascript

## Instructions
Your task is to make a function that can take any non-negative integer as an argument and return it with its digits in descending order. Essentially, rearrange the digits to create the highest possible number.

Examples:
```
Input: 42145 Output: 54421
Input: 145263 Output: 654321
Input: 123456789 Output: 987654321
```
✒️ FUNDAMENTALS

## Mon code
```js
class SmallestIntegerFinder {
  findSmallestInt(args) {
    return args.sort((a,b)=>a-b)[0];    
  }
}
```

## Code de la communauté
```js
class SmallestIntegerFinder {
  findSmallestInt(args) {
    return Math.min(...args)
  }
}
```

## Docs
- Arrays.sort : https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Global_Objects/Array/sort
