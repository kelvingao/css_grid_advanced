# lesson 01_02
> The default width of any row or column created is **auto**, take a list of length values (em, px, %, fr, etc.)

```CSS
#app {
    display: grid;
    grid-template-columns: 5em 1fr 1fr;
}
```

> you can declare columns width and row heights with any mix of measurement units, like a 10 pixel column, 4 em column, a 20% of the total width of the grid column, and then this one, which is 50% of the total width of the viewport.
```CSS
#app {
    display: grid;
    grid-template-columns: 10px 4em 20% 50vm;
}
```

> CSS grid has two additional measurement units and tools: Fraction (fr) Unit and minmax() Function. The minmax() function defines a size range greater than or min endless than or equal to max.
```CSS
#app {
    display: grid;
    grid-template-rows: 1fr minmax(10em, 20em) 1fr;
}
```

> repeat() Notation. The repeat() notation repeats the provided pattern a specified number of times
```CSS
grid-template-columns: repeat(4, 1fr 10px);
```