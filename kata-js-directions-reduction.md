Kata JS : Directions reduction

## Instructions

## Mon code
```js
function dirReduc(arr){
    const opposites = {'NORTH': 'SOUTH', 'EAST': 'WEST', 'SOUTH': 'NORTH', 'WEST': 'EAST'};
  
    return arr.reduce((prev, cur) => (opposites[prev.slice(-1)] === cur ? prev.pop() : prev.push(cur), prev), [])
}
```

## Code de la communauté
```js
```

## Docs
- Array reduce : https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/Reduce
- Array push : https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/push
- Arra pop : https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/pop
- Soluce web : https://losseff.xyz/katas/021-directions-reduction/javascript/
