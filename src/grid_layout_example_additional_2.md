# Grid panaudojimo pavyzdis (papildomi nustatymai II)

Galima tiesiogine tuo žodžio prasme nupaišyti mūsų layout naudojant `grid-template-areas` ir `grid-area`.

```css
body {
  display: grid;
  grid-template-rows: 150px auto 100px;
  grid-template-columns: minmax(200px, 3fr) 9fr;
  grid-template-areas: "header header"
                       "nav    content"
                       "nav    footer";
}
header {
  grid-area: header;
}
nav {
  grid-area: nav;
}
```
