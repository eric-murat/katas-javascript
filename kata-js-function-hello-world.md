# kata-js-find_unique
Kata JS : function hello world : https://www.codewars.com/kata/585d7d5adb20cf33cb000235

## Instructions
Make a simple function called greet that returns the most-famous "hello world!".  
Sure, this is about as easy as it gets. But how clever can you be to create the most creative hello world you can think of? What is a "hello world" solution you would want to show your friends?  
✒️ FUNDAMENTALS, FUNCTIONS, CONTROL FLOW, BASIC LANGUAGE FEATURES

## Mon code
```js
function greet() {
  return "hello world!";
}
```

## Solution de la communauté
```js
function findUniq(arr) {
  return arr.find(n => arr.indexOf(n) === arr.lastIndexOf(n));
}
```

## Docs
