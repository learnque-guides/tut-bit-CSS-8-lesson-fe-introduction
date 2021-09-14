# Grid panaudojimo pavyzdis II

Sukurkime index.html ir pabandykime sudėti hml elementus, kurie nusakytų mūsų šabloną.

```html
<!DOCTYPE html>
<head>
    <style>

    </style>
</head>
<body>
  <header></header>
  <nav></nav>
  <main></main>
  <footer></footer>
</body>
```

Savo css mes pradedame rašyti išplėčiant `body` tag, taip ji paversdami `grid` kontaineriu.

```css
html, body {
  width: 100vw;
  min-height: 100vh;
  margin: 0;
  padding: 0;
}
body {
  display: grid;
}
```

Dabar mes jau naudojam CSS grid.
