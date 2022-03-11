Kata JS : Give me a diamond 

## Instructions

## Mon code
```js
function diamond(n){
  if ((n%2 == 0) || (n <= 0)) {
    return null;
  }
  var res = "";
  var milieu = (n+1) / 2;
  // Parcours des lignes
  for (var i = 1; i <= n; i++) {
    // Lignes basses
    if (i < milieu) {
      // Espaces vides
      for (var j = 0; j < (milieu - i); j++) {
        res = res + ' ';
      }
      // Etoiles
      for (var jj = 0; jj < ((i * 2) -1); jj++) {
        res = res + '*';
      }
    }
    // Ligne du milieu
    if (i == milieu) {
      for (var k = 0; k < n; k++) {
        res = res + '*';
      }
    }
    // Lignes hautes
    if (i > milieu) {
      // Espaces vides
      for (var l = 0; l < (i - milieu); l++) {
        res = res + ' ';
      }
      // Etoiles
      for (var ll = 0; ll < (((n+1 -i) * 2) -1); ll++) {
        res = res + '*';
      }
    }
    
    res = res + '\n';
  }
  return res;
}
```

## Code de la communauté
```js
var diamond = n => {
  if(isNaN(n) || n < 1 || !(n % 2)) return null;
  var line = i => Array.apply(0, Array((n - i) / 2 + 1)).join(' ') + Array.apply(0, Array(i + 1)).join('*'),
      top = Array.apply(0, Array(Math.floor(n / 2))).map((v, i) => line(i * 2 + 1));
  return top.join('\n') + '\n' + line(n) + '\n' + top.slice().reverse().join('\n') + '\n';
};
```

## Docs
