Kata JS : Calculating with functions https://www.codewars.com/kata/525f3eda17c7cd9f9e000b39

## Instructions
This time we want to write calculations using functions and get the results. Let's have a look at some examples:
```
seven(times(five())); // must return 35
four(plus(nine())); // must return 13
eight(minus(three())); // must return 5
six(dividedBy(two())); // must return 3
```
Requirements:
- There must be a function for each number from 0 ("zero") to 9 ("nine")
- There must be a function for each of the following mathematical operations: plus, minus, times, dividedBy
- Each calculation consist of exactly one operation and two numbers
- The most outer function represents the left operand, the most inner function represents the right operand
- Division should be integer division. For example, this should return 2, not 2.666666...:
```
eight(dividedBy(three()));
```
✒️ FUNDAMENTALS, FUNCTIONS, CONTROL FLOW, BASIC LANGUAGE FEATURES, FUNCTIONAL PROGRAMMING, DECLARATIVE PROGRAMMING, HIGHER-ORDER FUNCTIONS

## Mon code
```js
function zero() { return arguments.length === 1 ? arguments[0](0) : 0; }
function one() { return arguments.length === 1 ? arguments[0](1) : 1; }
function two() { return arguments.length === 1 ? arguments[0](2) : 2; }
function three() { return arguments.length === 1 ? arguments[0](3) : 3; }
function four() { return arguments.length === 1 ? arguments[0](4) : 4; }
function five() { return arguments.length === 1 ? arguments[0](5) : 5; }
function six() { return arguments.length === 1 ? arguments[0](6) : 6; }
function seven() { return arguments.length === 1 ? arguments[0](7) : 7; }
function eight() { return arguments.length === 1 ? arguments[0](8) : 8; }
function nine() { return arguments.length === 1 ? arguments[0](9) : 9; }

function plus(val) {
  return function(left) {
    return left + val;
  }
}
function minus(val) {
  return function(left) {
    return left - val;
  }
}
function times(val) {
  return function(left) {
    return left * val;
  }
}
function dividedBy(val) {
  return function(left) {
    // Division entière
    return Math.floor(left / val);
  }
}
```

## Code de la communauté
```js
var n = function(digit) {
  return function(op) {
    return op ? op(digit) : digit;
  }
};
var zero = n(0);
var one = n(1);
var two = n(2);
var three = n(3);
var four = n(4);
var five = n(5);
var six = n(6);
var seven = n(7);
var eight = n(8);
var nine = n(9);

function plus(r) { return function(l) { return l + r; }; }
function minus(r) { return function(l) { return l - r; }; }
function times(r) { return function(l) { return l * r; }; }
function dividedBy(r) { return function(l) { return l / r; }; }
```

## Docs
- Math floor (division entière) : https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Global_Objects/Math/floor
