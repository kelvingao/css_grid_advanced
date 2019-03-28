# lesson 01_03: Manual grid item placement
> Places the item by declaring the start and end lines, the other grid items will flow up to take up to the new, available space

```CSS
.masthead {
  grid-column: 2/4;
  grid-row: 2/3;
}
```
> Implicit Lines. If grid item placement requires additional columns or rows to be created, the browser adds implicit lines to keep the grid structurally sound.
```CSS
.footer-content {
  grid-column: 1/4;
  grid-row: 4;
}
```