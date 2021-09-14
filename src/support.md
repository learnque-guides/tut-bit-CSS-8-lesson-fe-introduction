# CSS3 @supports

Kartu su CSS3 atsirado, @supports, kuris leidžia patikrinti ar naujas funkcionalumas yra palaikomas naršyklėje (vadinamas *feature query*) ir jei palaikomas tai, tada CSS taisyklė/funkcionalumas pritaikomas.

Sintaksė:

```css
@supports (display: grid) {
  div {
    display: grid;
  }
}

@supports not (display: grid) {
  div {
    float: right;
  }
}

@supports not (not (transform-origin: 2px))

@supports (display: grid) and (not (display:inline-grid))
```

