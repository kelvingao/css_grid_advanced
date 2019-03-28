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
}
</style>
