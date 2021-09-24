# FR unit, auto-rows, repeat() and minmax()

*Kai naudojame CSS grid ir nusakome eilutes (ang. columns) arba stulpelius (ang. rows) tai toks veiksmas vadinamas `set of tracks`.*

* Large grids with many tracks can use the repeat() notation, to repeat all or a section of the track listing.
* Tracks can be defined using any length unit. Grid also introduces an additional length unit to help us create flexible grid tracks. The new `fr` unit represents a fraction of the available space in the grid container.
* You can also define a set size for tracks created in the implicit grid with the grid-auto-rows and grid-auto-columns properties.
* When setting up an explicit grid or defining the sizing for automatically created rows or columns we may want to give tracks a minimum size, but also ensure they expand to fit any content that is added. Grid has a solution for this with the minmax() function.



```css
.wrapper {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    grid-template-columns: repeat(3, 1fr);
    grid-auto-columns: 1fr;
    grid-auto-rows: 200px;
    grid-auto-rows: minmax(100px, auto);
}
```
 