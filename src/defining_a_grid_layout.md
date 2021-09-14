# Grid apibrėžimas

* `display` nurodome, kad naudosime `grid` layout mūsų kontaineryje.
* Naudojant grid layout, mes nurodome viena iš ašių su `grid-template-columns` (y ašis) arba `grid-template-rows` (x ašis) ir tada nurodome kaip kontentas (elementai) turi pasikartoti (koks turi būti jų dydis, pavyzdžiui, aukštis). 
* Galima naudoti ir `grid-auto-rows`, `grid-auto-columns` ir `grid-auto-flow`. Jie skiriasi nuo ankščiau minėtu tuom, kad visiems elementams yra nusakomas dydis, o ne atskirai.
* Yra galimybė naudoti tik `grid` property, kuri dar vadinama shorthand property. Joje galima nusakyti kitų (anksčiau minėtų) properčių dydžius vienu metu.

<style>
    .interactive {
        background-color: #f4f4f4;
        border: 1px solid #d5d5d5;
        color: #1b1b1b;
        padding: 10px;
        width: 100%;
    }
</style>

---

<iframe class="interactive" height="390" src="https://interactive-examples.mdn.mozilla.net/pages/css/grid-template-rows.html" title="MDN Web Docs Interactive Example" loading="lazy">
</iframe>

---

<iframe class="interactive" height="390" src="https://interactive-examples.mdn.mozilla.net/pages/css/grid-template-columns.html" title="MDN Web Docs Interactive Example" loading="lazy">
</iframe>

---

<iframe class="interactive" height="390" src="https://interactive-examples.mdn.mozilla.net/pages/css/grid-auto-columns.html" title="MDN Web Docs Interactive Example" loading="lazy">
</iframe>

---

<iframe class="interactive" height="390" src="https://interactive-examples.mdn.mozilla.net/pages/css/grid-auto-rows.html" title="MDN Web Docs Interactive Example" loading="lazy">
</iframe>

---

<iframe class="interactive" height="390" src="https://interactive-examples.mdn.mozilla.net/pages/css/grid-auto-flow.html" title="MDN Web Docs Interactive Example" loading="lazy">
</iframe>

---

<iframe class="interactive" height="390" src="https://interactive-examples.mdn.mozilla.net/pages/css/grid.html" title="MDN Web Docs Interactive Example" loading="lazy">
</iframe>

---

```css
div {
    /* <'grid-template'> values */
    grid: none;
    grid: "a" 100px "b" 1fr;
    grid: [linename1] "a" 100px [linename2];
    grid: "a" 200px "b" min-content;
    grid: "a" minmax(100px, max-content) "b" 20%;
    grid: 100px / 200px;
    grid: minmax(400px, min-content) / repeat(auto-fill, 50px);

    /* <'grid-template-rows'> /
    [ auto-flow && dense? ] <'grid-auto-columns'>? values */
    grid: 200px / auto-flow;
    grid: 30% / auto-flow dense;
    grid: repeat(3, [line1 line2 line3] 200px) / auto-flow 300px;
    grid: [line1] minmax(20em, max-content) / auto-flow dense 40%;

    /* [ auto-flow && dense? ] <'grid-auto-rows'>? /
    <'grid-template-columns'> values */
    grid: auto-flow / 200px;
    grid: auto-flow dense / 30%;
    grid: auto-flow 300px / repeat(3, [line1 line2 line3] 200px);
    grid: auto-flow dense 40% / [line1] minmax(20em, max-content);

    /* Global values */
    grid: inherit;
    grid: initial;
    grid: revert;
    grid: unset;
}
```
---