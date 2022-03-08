Kata JS : Number of people in the bus

## Instructions

## Mon code
```js
var number = function(busStops){
  return busStops.reduce(function(sum, n){
    return (n[0] - n[1]) + sum;
  }, 0)
}
```

## Code de la communauté
```js
```

## Docs
- Array reduce :
