<template>
  <div id="app">
    <header-box :navList="this.navbarList" :logoString="this.navbarLogo"/>
    <main-box />
    <footer-box />
  </div>
</template>

<script>
import HeaderBox from './components/HeaderBox.vue'
import MainBox from './components/MainBox.vue'
import FooterBox from './components/FooterBox.vue'

export default {
  name: 'App',
  components: {
    HeaderBox,
    MainBox,
    FooterBox,
  },
  data() {
    return {
      // header data
      navbarList: [
        'Home',
        'Pages',
        'Courses',
        'Features',
        'Blog',
        'Shop',
      ],
      navbarLogo: 'light-logo'
    }
  }
}
</script>

<style lang="scss">
  @import './style/app.scss'
</style>
