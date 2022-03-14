Kata JS : Longest Palyndrom : 

## Instructions

## Mon code
```js
longestPalindrome=function(s){
  var res = 0;
  var resBis = 0;
  var resFinal = 1;
  var arr = s.split('');
  // Cas particulier 1 caractère
  if (s.length == 1) return 1;
  // Cas particulier 2 caractères
  if (s.length == 2) return arr[0] == arr[1] ? 2 : 0;
  // Boucle sur chaque caractère
  var m1, m2;
  for (var i = 0; i < arr.length; i++) {
    // On compare les 2 morceaux
    m1 = arr.slice(i);
    m2 = arr.slice(0,i).reverse();
    console.log(m1)
    console.log(m2)
    // Parcours "pair"
    res = 0;
    for (var j = 0; j < Math.min(m1.length, m2.length); j++) {
      if (m1[j] == m2[j]) {
        res = res +2;
      } else {
        break;
      }
    }
    
    // Parcours "impair"
    resBis = 1;
    m2 = m2.slice(1, m2.length);
    for (var j = 0; j < Math.min(m1.length, m2.length); j++) {
      if (m1[j] == m2[j]) {
        resBis = resBis +2;
      } else {
        break;
      }
    }

    // Résultat final
    resFinal = Math.max(Math.max(res, resBis), resFinal);
  }
  return resFinal;
}```

## Code de la communauté
```js
```

## Docs
