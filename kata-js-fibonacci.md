Kata JS : Product of consecutive Fib numbers

## Instructions

## Mon code
```js
function productFib(prod){
  var res = [];
  
  for (var i = 0; fib(i) * fib(i+1) <= prod; i++) {
    if (fib(i) * fib(i+1) == prod) {
      res.push(fib(i));
      res.push(fib(i+1));
      res.push(true);
      return res;
    } else if ((fib(i) * fib(i+1) < prod) && (fib(i+1) * fib(i+2) > prod)) {
      res.push(fib(i+1));
      res.push(fib(i+2));
      res.push(false);
      return res;
    }
  }
  return res;
}

function fib(n) {
  if (n < 2) {
    return 1;
  } else {
    return fib(n-1) + fib(n-2);
  }
}
```

## Code de la communauté
```js
```

## Docs
