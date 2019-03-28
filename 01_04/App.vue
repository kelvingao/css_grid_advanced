<template lang='pug'>
  #app
    a.skip-link.screen-reader-text(href='#content') Skip to content
    header.masthead
      code.identifier
        pre .masthead      
      h2 CSS Grid
    // .masthead
    div.page-title
      code.identifier
        pre .page-title      
      h1 Demo sandbox for Advanced Layouts with CSS Grid
    // .page-title
    main#content.main-content
      code.identifier
        pre .main-content      
      h2 Main content
      p This is where the main bulk of the document content would go.
    // #content .main-content
    aside.sidebar
      code.identifier
        pre .sidebar      
      h2 Sidebar
      p The place where things of less relevance appears.
    // .sidebar
    footer.footer-content
      code.identifier
        pre .footer-content      
      h2 Footer
      p
        span.bg The place where site nav and other meta info typically appears.
    // .footer-content

</template>

<script>

export default {
  name: 'app',
 
}
</script>

<style>
#app {
  display: grid;
  grid-template-columns: [main-start] 2fr [main-end] 1fr [sidebar-start] 1fr [sidebar-end];
  grid-template-rows: auto 1fr 3fr;
}
.masthead {
  grid-column: main-end/sidebar;
  grid-row: 2/3;
}
.page-title {
  grid-column: main/sidebar;
  grid-row: 1/2;
}
.main-content {
  grid-column: main;
  grid-row: 2/4;
}
.sidebar {
  grid-column: 2/4;
  grid-row: 3/4;
}
.footer-content {
  grid-column: 1/4;
  grid-row: 4;
}
</style>
