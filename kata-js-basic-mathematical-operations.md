Kata JS : Basic Mathematical Operations

## Mon code
```js
function basicOp(operation, value1, value2) {
  switch (operation) {
    case '+':
      return Number(value1) + Number(value2);
    case '-':
      return Number(value1) - Number(value2);
    case '*':
      return Number(value1) * Number(value2);
    case '/':
      return Number(value1) / Number(value2);
  default:
    return "Sorry, operation incorrect : " + operation;
  }
}
```

## Code de la communauté
```js
function basicOp(operation, value1, value2)
{
  return eval(value1 + operation + value2);
}
```

## Docs
- switch : https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/switch
- eval : https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/eval
