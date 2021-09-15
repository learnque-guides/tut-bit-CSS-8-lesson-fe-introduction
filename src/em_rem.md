# Em vs rem

<cite>
Ems, the most common relative length unit, are a measure used in typography, referring to a specified font size. In CSS, 1 em means the font size of the current element; its exact value varies depending on the element you’re applying it to.
</cite>

```html
<!doctype html>
<head>
  <style>
  body {
    font-size: 16px;
  }

  .slogan {
    font-size: 1.2em;
  }
  </style>
</head>

<body>
  We love coffee
  <p class="slogan">We love coffee</p>
</body>
```

```html
<!doctype html>
<head>
  <style>
  body {
    font-size: 16px;
  }

  .slogan {
    font-size: 1.2em;
    padding: 1.2em;
    background-color: #ccc;
  }
  </style>
</head>

<body>
  <p class="slogan">We love coffee</p>
</body>
```

---

<cite>
Rem is short for root em. Instead of being relative to the current element, rems are relative to the root element. No matter where you apply it in the document, 1.2 rem has the same computed value: 1.2 times the font size of the root element. The following listing establishes the root font size and then uses rems to define the font size for unordered lists relative to that.
</cite>

```css
<!doctype html>
<head>
  <style>
  body {
    font-size: 16px;
  }

  .slogan {
    font-size: 1.2rem;
    padding: 1.2rem;
    background-color: #ccc;
  }
  </style>
</head>

<body>
  <p class="slogan">We love coffee</p>
</body>

```

---

<cite>
My default is to use rems for font sizes, pixels for borders, and ems for most other measures, especially paddings, margins, and border radius (though I favor the use of percentages for container widths when necessary).
</cite>