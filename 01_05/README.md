# lesson 01_05: Grid areas
> **grid-template-areas** is applied to grid container, uses a text-based grid map to apply grid area names to individual cells.
```CSS
#app {
  display: grid;
  grid-template-columns: 2fr 1fr 1fr;
  grid-template-rows: auto 1fr 3fr;
  grid-template-areas:
    "title title title"
    "main masthead masthead"
    "main sidebar footer";
}
```