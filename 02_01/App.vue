<template lang='pug'>
  #app
    a.skip-link.screen-reader-text(href='#content') Skip to content
    header.masthead
      div.logo    
      h2.site-title is for Grid
    // .masthead

    figure.feature
      img(src='./images/wing.jpg' alt='The sun sets behind the wing of an airliner.')

  
    main#content.main-area
      section.splash    
        div.splash-content
          h2.content-title Full Bleed CSS Grid
          div.splash-text
            p CSS Grid provides a trivial solution to a complex problem: How to display full-bleed content mixed with center-aligned width-constrained content. This solution ellimiates the need for auto-margins and floats while allowing the developer to change the grid globally and see those changes apply to each element individually.
      section.buckets
        ul
          li
            img(src='./images/nerve.jpg' alt='The leaves of a Nerve Plant.')
            div.bucket
              h3.bucket-title Grid is great
              p CSS Grid is a two-dimensional layout tool. It is great for laying out content in a grid, and for laying out content in two dimensions.
          li
            img(src='./images/tree.jpg' alt='A solitary tree in a field.')
            div.bucket
              h3.bucket-title Flex is great too
              p That said, Grid is not always the right option for layouts. If for example you need to lay out a series of identical boxes like those you see here, Flex may be a better option.
      section.more
        div.more-content
          h2.content-title Subgrid would be nice here
          p The solution provided here is limited by the lack of support for subgrids. If subgrids were available, the solution would be more refined. In lieu of subgrid, the solution applies a grid to each full-bleed section within the layout using a common class <code>.grid</code> and creates the full-bleed/centered effect that way. 
    // main#content.main-area

    aside.sidebar
      div.twin
        h2.content-title Grid lets you do unusual things      
        p Creating this layout, where two items share the total available viewport width evenly alongside full-width and centered content, is suprisingly complex if you don't have CSS Grid available.
      div.twin
        h2.content-title Grid requires a rethink      
        p Seeing this layout you may still think it's better to just use old methods with auto-margins and max-widths. And you <em>can</em>, but looking at the CSS you'll see the Grid approach is both cleaner and easier to understand.
    // .sidebar

    footer.colophon
      aside
        | All photos: 
        a(href='#', target='_blank', rel='nofollow') Some one
      aside
        | For more information, visit 
        a(href='#', target='_blank', rel='nofollow') Some where
    // .footer-content

</template>

<script>

export default {
  name: 'app',
 
}
</script>

<style>

</style>
