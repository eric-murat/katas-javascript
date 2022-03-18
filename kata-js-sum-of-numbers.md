Kata JS : Sum of Numbers 

## Instructions

## Mon code
```js
function getSum( a,b ) {
  var tab = [a,b].sort((a,b)=>a-b);
  var res = 0;
  for (var i = tab[0]; i <= tab[1]; i++) {
    res = res + i;
  }
  return res;
}
```

## Docs
- Array sort :
- Array reduce :
