<template>
  <div id="app">
    <header-box :navList="this.navbarList" 
      :logoString="this.navbarLogo"/>

    <main-box :stats="stats"
      :blogs="blogs"
      :courses="courses"
      :sponsors="sponsors"
      :helpInfos="helpInfos"/>

    <footer-box :street="this.addressData.street" 
      :number="this.addressData.number" 
      :email="this.addressData.email"
      :exploreLinks="this.explore"
      :informationLinks="this.information"
      :socialIcons="socialIcons"/>
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
      // header data --------------------------------------------------------------------
      navbarList: [
        {
          name: 'Home',
          link: '#/'
        },
        {
          name: 'Pages',
          link: '#/'
        },
        {
          name: 'Courses',
          link: '#/'
        },
        {
          name: 'Features',
          link: '#/'
        },
        {
          name: 'Blog',
          link: '#/'
        },
        {
          name: 'Shop',
          link: '#/'
        },
      ],
      navbarLogo: 'light-logo',
      // footer data --------------------------------------------------------------------
      addressData: {
        street: '382 NE 191st St # 87394 Miami, FL-33179-3899',
        number: '+1(305)547-9909(9am-5pm EST, Monday-Friday)',
        email: 'support@maxcoach.com'
      },
      socialIcons: [
        {
          icon: 'fab fa-facebook-square',
          link: '#/'
        },
        {
          icon: 'fab fa-twitter',
          link: '#/'
        },
        {
          icon: 'fab fa-instagram',
          link: '#/'
        },
        {
          icon: 'fab fa-linkedin',
          link: '#/'
        },
      ],
      explore: [
        {
          name: 'Start here',
          link: '#/',
        },
        {
          name: 'Success story',
          link: '#/',
        },
        {
          name: 'Blog',
          link: '#/',
        },
        {
          name: 'Courses',
          link: '#/',
        },
        {
          name: 'About us',
          link: '#/',
        },
        {
          name: 'Contact us',
          link: '#/',
        },
      ],
      information: [
        {
          name: 'Membership',
          link: '#/',
        },
        {
          name: 'Puchase guide',
          link: '#/',
        },
        {
          name: 'Privacy policy',
          link: '#/',
        },
        {
          name: 'Terms of services',
          link: '#/',
        },
      ],
      // main data --------------------------------------------------------------------------
      // part one stats data
      stats: [
        {
          data: 'FINISHED SESSIONS',
          number: '1.926'
        },
        {
          data: 'ENROLLED LEARNERS',
          number: '3.092+'
        },
        {
          data: 'ONLINE INSTRUCTORS',
          number: '200'
        },
        {
          data: 'SATISFACTION RATE',
          number: '100%'
        },
      ],
      // part three courses data
      courses: [
        {
          price: '$40.00',
          course_name: 'Learning to Write as a Professional Author',
          lessons: 20,
          students: 50,
          course_image: 'course-02-480x298.jpg'
        },
        {
          price: 'Free',
          course_name: 'Customer-centric Info-Tech-Strategies',
          lessons: 24,
          students: 24,
          course_image: 'stock-full-hd-03-480x298.jpg'
        },
        {
          price: '$19.00',
          course_name: 'Open Programming Courses for Everyone: Python',
          lessons: 17,
          students: 62,
          course_image: 'stock-full-hd-04-480x298.jpg'
        },
        {
          price: '$26.00',
          course_name: 'Academic Listening and Note-taking',
          lessons: 14,
          students: 67,
          course_image: 'stock-full-hd-06-480x298.jpg'
        },
        {
          price: '$39.00',
          course_name: 'Master jQuery in a Short Periodo of Time',
          lessons: 6,
          students: 51,
          course_image: 'course-featured-image-01-480x298.jpg'
        },
        {
          price: '$59.00',
          course_name: 'Introduction to Javascript for Beginners',
          lessons: 14,
          students: 76,
          course_image: 'stock-full-hd-05-480x298.jpg'
        },
      ],
      // part four sponsor/client data
      sponsors: [
        {
          name: 'AQUA',
          client_image: 'client-logo-colored-01.png'
        },
        {
          name: 'AdRoll',
          client_image: 'client-logo-colored-02.png'
        },
        {
          name: 'FireFox',
          client_image: 'client-logo-colored-03.png'
        },
        {
          name: 'WoodLand',
          client_image: 'client-logo-colored-04.png'
        },
        {
          name: 'BullFit',
          client_image: 'client-logo-colored-05.png'
        },
        {
          name: 'SixBase',
          client_image: 'client-logo-colored-06.png'
        },
      ],
      // part five blogs data
      blogs: [
        {
          thumbnail: 'artist-blog-01-480x325.jpeg',
          author: 'ARTIST',
          title: 'Brush Strokes Energize Trees in Paintings',
          date: 'May 15, 2020',
          views: 688
        },
        {
          thumbnail: 'artist-blog-02-480x325.jpg',
          author: 'ARTIST',
          title: 'Pocket-Sized Notebooks Hold Miniature Paintings',
          date: 'May 15, 2020',
          views: 603
        },
        {
          thumbnail: 'artist-blog-03-480x325.jpg',
          author: 'ARTIST',
          title: 'Connection Between Self-Portrait and Identity',
          date: 'May 15, 2020',
          views: 397
        },
      ],
      helpInfos: [
        {
          icon: 'far fa-flag',
          title: 'Idea Discussion',
          info: 'Get teamed up with the specialists who work and teach coding for years at famous universities.',
        },
        {
          icon: 'fas fa-cog',
          title: 'Web Development',
          info: 'Lear to start building a webpage from scratch. You decide your own pace, course and speed.',
        },
        {
          icon: 'far fa-life-ring',
          title: 'System Administration',
          info: 'Learnes are encouraged to study the mechanism and structure of system administration.',
        },
        {
          icon: 'fas fa-desktop',
          title: 'Graphic Design',
          info: 'Have passion for graphics and arts? Show your talent with confidence and self-assertiveness.',
        },
      ],
    }
  }
}
</script>

<style lang="scss">
  @import './style/app.scss';
</style>
