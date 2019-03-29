# lesson 02_01: Created the main grid
> just like in other web design, we're going to start mobile first and scale the viewport up and then find out where the natural break points are four our grid.
```CSS
@supports (grid-area: auto) {
  @media screen and (min-width: 50em) {
    #app {
      max-width: none;
      display: grid;
      grid-template-columns: 15em auto;
    }
  }
}
```