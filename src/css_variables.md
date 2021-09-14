# CSS variables

CSS leidžia mums nusakyti savo kintamuosius, naudojant sintaksę

```css
/* Variable is defined in element scope  */
element {
    --name-color: black;
}

/* Variable is defined in global scope */
:root {
    --name-color
}
```

Kintamasis gali būti panaudotas su funkcija `var()`

```css
div {
    color: var(--name-color);
}
```
