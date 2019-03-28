# lesson 01_04: Named lines
> The name of each line goes inside square brackets and here you can give the lines any name you want as long as you use hyphens instead of spaces. 
```CSS
#app {
  display: grid;
  grid-template-columns: [main-start] 2fr [main-end] 1fr [sidebar-start] 1fr [sidebar-end];
  grid-template-rows: auto 1fr 3fr;
}
```
>  There's built in short hand naming convention for named lines that you can use to simplify, but you can not give one line two different names.
```CSS
.masthead {
  grid-column: main-end/sidebar;
  grid-row: 2/3;
}

.main-content {
  grid-column: main;
  grid-row: 2/4;
}
```