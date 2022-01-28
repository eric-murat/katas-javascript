# kata-js-regex-validate-PIN-code
Kata JS : Regex validate PIN code

# Instructions
ATM machines allow 4 or 6 digit PIN codes and PIN codes cannot contain anything but exactly 4 digits or exactly 6 digits.
If the function is passed a valid PIN string, return true, else return false.

Examples (Input --> Output)
```
"1234"   -->  true
"12345"  -->  false
"a234"   -->  false
```
✒️FUNDAMENTALS, REGULAR EXPRESSIONS

# Mon code
```js
function validatePIN (pin) {
  // Expression régulière 4 ou 6 digits
  return /^(\d{4}|\d{6})$/.test(pin);
}
```

# Références :
- RegEx : https://developer.mozilla.org/fr/docs/Web/JavaScript/Reference/Global_Objects/RegExp
- Stack Overflow : https://stackoverflow.com/questions/49179722/regex-validate-pin-code-js
