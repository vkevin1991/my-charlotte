<template lang="pug">
div.columns
  div.column.is-12
    div.columns
      div.column.is-10
        h1.card-header-title
          | Charlotte, Walden's Bot
      div.column.is-2
        span.icon
          i.fas.fa-angle-down(aria-hidden='true')
    hr
    div.columns
      div.column.is-2
        a.card-header-icon(href='#', aria-label='more options')
            span.icon
              i.fas.fa-angle-down(aria-hidden='true')
      div.column.is-10
        div.card
          header.card-header
            p.card-header-title
              | 01/01/2018
          .card-content
            .content
              | Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus nec iaculis mauris.
    div.columns
      div.column.is-2
        a.card-header-icon(href='#', aria-label='more options')
            span.icon
              i.fas.fa-angle-down(aria-hidden='true')
      div.column.is-10
        div.card
          header.card-header
            p.card-header-title
              | 01/01/2018
          .card-content
            .content
              | Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus nec iaculis mauris.
    div.columns
      div.column.is-9.is-offset-3
        div.card
          header.card-header
            p.card-header-title
              | 01/01/2018
          .card-content
            .content
              | Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus nec iaculis mauris.
    div.columns
      div.column.is-12
        .field
          .control
            input.input(type='text', placeholder='Primary input')
</template>
<script>
export default {}
</script>
<style lang="scss" scoped>
  $column-gap:0;
  hr{
    margin-top: 0;
  }
</style>
