Kata JS : Basic Mathematical Operations

## Instructions
Your task is to create a function that does four basic mathematical operations.

The function should take three arguments - operation(string/char), value1(number), value2(number).  
The function should return result of numbers after applying the chosen operation.

Examples(Operator, value1, value2) --> output
```
('+', 4, 7) --> 11
('-', 15, 18) --> -3
('*', 5, 5) --> 25
('/', 49, 7) --> 7
```
✒️ FUNDAMENTALS, MATHEMATICS, ALGORITHMS, NUMBERS, OPERATORS

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
