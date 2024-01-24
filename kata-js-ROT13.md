```js
function rot13(str) {
  let result = "";
  let charCode;
  for (let i=0; i < str.length; i++) {
    charCode = str.charCodeAt(i);
    // Caractères majuscules
    if (charCode >= 65 && charCode <= 90) {
      charCode = 65 + (charCode - 65 + 13) % 26;
    } else if (charCode >= 97 && charCode <= 122) {
    // Caractères minuscules
      charCode = 97 + (charCode - 97 + 13) % 26;
    }
    result = result + String.fromCharCode(charCode);
  }
  return result;
}
```
