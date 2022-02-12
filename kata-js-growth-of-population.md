Kata JS : Growth of a population

## Instructions

## Mon code
```js
function nbYear(p0, percent, aug, p) {
    // Population initiale
    var popI = p0;
    // Boucle sur les années
    for(var i = 0; popI < p;i++) {
      popI = popI + popI * percent / 100 + aug;
    }
    return i;
}
```

## Code de la communauté
```js
```

## Docs
