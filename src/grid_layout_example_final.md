# Grid panaudojimo pavyzdis final

```html
<!DOCTYPE html>
<head>
    <style>
        html, body {
            width: 100vw;
            min-height: 100vh;
            margin: 2px;
            padding: 0;
        }

        body {
            display: grid;
            grid-template-rows: 150px auto 100px;
            grid-template-columns: minmax(200px, 3fr) 9fr;
        }

        body > * {
            border: 1px solid green;
        }

        header {
            grid-column: 1 / 3;
        }

        nav {
            grid-row: 2 / span 2;
        }
    </style>
</head>
<body>
  <header>Header</header>
  <nav>Nav</nav>
  <main>Contant</main>
  <footer>Footer</footer>
</body>
```