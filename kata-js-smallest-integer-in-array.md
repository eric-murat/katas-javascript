Kata JS : Smallest integer in array :

## Instructions

## Mon code
```js
class SmallestIntegerFinder {
  findSmallestInt(args) {
    return args.sort((a,b)=>a-b)[0];    
  }
}
```

## Code de la communaut√©
```js
class SmallestIntegerFinder {
  findSmallestInt(args) {
    return Math.min(...args)
  }
}
```

## Docs
