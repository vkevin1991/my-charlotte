<template lang="pug">
section.section
  div.columns
    app-sidebar
    app-content
    app-footer
  section(v-bind:class="classPanel")
    right-panel
</template>
<script>
import Container from './Container'
import SideBar from './SideBar'
import Footer from './Footer'
import RightPanel from './RightPanel'
export default {
  name: 'Layout',
  data () {
    return {
      classPanel: {
        'is-open': true,
        'box': true,
        'right-panel': true
      },
      msg: 'Welcome to Your Vue.js App'
    }
  },
  components: {
    'app-sidebar': SideBar,
    'app-content': Container,
    'right-panel': RightPanel,
    'app-footer': Footer
  }
}
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
html, body, #app {
  height: 100%;
}
#app {
  min-height: 100%;
}

.footer {
  margin-top: -12px;
}
@media screen and (max-width: 768px) {
  #menu-toggle:checked + .nav-menu {
    display: block;
  }
}
section.right-panel{
  position: fixed;
  height: 100%;
  width: 400px;
  right: 0;
  top: 0;
  bottom: 0;
  z-index: 3;
  visibility: hidden;
}

section.right-panel.is-open{
  visibility: visible;
}

</style>
