
```js no-beautify
"" + 1 + 0 = "10" // (1)
"" - 1 + 0 = -1 // (2)
true + false = 1
6 / "3" = 2
"2" * "3" = 6
4 + 5 + "px" = "9px"
"$" + 4 + 5 = "$45"
"4" - 2 = 2
"4px" - 2 = NaN
7 / 0 = Infinity
" -9\n" + 5 = " -9\n5"
" -9\n" - 5 = -14
null + 1 = 1 // (3)
undefined + 1 = NaN // (4)
```

1. Adunarea cu un string `"" + 1` convertește `1` la string: `"" + 1 = "1"`, și apoi avem `"1" + 0`, aceleași reguli sunt aplicate.
2. Scăderea `-` (ca majoritatea operațiilor matematice) funcționeză doar cu numere, convertește un string gol `""` la `0`.
3. `null` devine `0` după conversia numerică.
4. `undefined` devine `NaN` după conversia numerică.