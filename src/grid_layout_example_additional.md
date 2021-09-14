# Grid panaudojimo pavyzdis (papildomi nustatymai I)

```css
body {
  display: grid;
  grid-template-rows: 150px [nav-start] auto 100px [nav-end];
  grid-template-columns: [header-start] minmax(200px, 3fr) 9fr [header-end];
}
header {
  grid-column: header-start / header-end;
}
nav {
  grid-row: nav-start / nav-end;
}
```
Mes nurodome tiesiogiai kur turi prasidėti ir kur tūri baigtis elementas (header arba nav).