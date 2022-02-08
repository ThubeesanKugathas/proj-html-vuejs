<template>
  <div id="app">
    <header-box :navList="this.navbarList" :logoString="this.navbarLogo"/>
    <main-box />
    <footer-box :street="this.addressData.street" 
      :number="this.addressData.number" 
      :email="this.addressData.email"
      :exploreLinks="this.explore"
      :informationLinks="this.information"/>
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
      navbarLogo: 'light-logo',
      // footer data
      addressData: {
        street: '382 NE 191st St # 87394 Miami, FL-33179-3899',
        number: '+1(305)547-9909(9am-5pm EST, Monday-Friday)',
        email: 'support@maxcoach.com'
      },
      explore: [
        'Start here',
        'Success story',
        'Blog',
        'Courses',
        'About us',
        'Contact us'
      ],
      information: [
        'Membership',
        'Puchase guide',
        'Privacy policy',
        'Terms of services'
      ],
    }
  }
}
</script>

<style lang="scss">
  @import './style/app.scss'
</style>
