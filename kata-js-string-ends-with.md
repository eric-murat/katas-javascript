Kata JS : String ends with 

## Instructions

## Mon code
```js
function solution(str, ending){
  return ending.length <= 0 ? true : ending == str.slice(-1 * ending.length);
}
```

## Code de la communauté
```js
```

## Docs
- Array slice : https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/slice
