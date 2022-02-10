<template>
    <header class="u_d-flex u_position-relative">
        <!-- Background waves repeated trough v-for -->
        <div class="u_d-flex u_position-absolute wave small-box">
            <img v-for="(image, i) in 2" :key="i" class="small" src="../assets/jumbotron-background-wave-small.svg" alt="small wave">
        </div>
        <div class="u_d-flex u_position-absolute wave medium-box">
            <img v-for="(image, i) in 2" :key="i" class="medium" src="../assets/jumbotron-background-wave-medium.svg" alt="medium wave">
        </div>
        <div class="u_d-flex u_position-absolute wave big-box">
            <img v-for="(image, i) in 2" :key="i" class="big" src="../assets/jumbotron-background-wave-big.svg" alt="big wave">
        </div>

        <!-- container of navbar, button, title -->
        <div class="u_container container">
            <header-nav-box :navList="navList" :logoString="logoString"/>
            <div class="u_text-centered header-title">
                <h2>Learn At Your Own Pace!</h2>
                <p>Get teamed up with people of same will</p>
                <div class="u_d-inline-block u_pointer header-button">Get started for free</div>
            </div>
            <!-- three images in center-bottom of headerbox -->
            <div class="u_d-flex u_justify-center header-images">
                <img src="../assets/home-6-hero-left-person.png" alt="left-person">
                <img id="center-image" src="../assets/video-screen.png" alt="video-screen">
                <img id="right-image" src="../assets/home-6-hero-right-person.png" alt="right-person">
            </div>
        </div>

        <div class="u_d-flex u_position-fixed icon-fixed">
            <i class="u_pointer fas fa-ruler"></i>
            <i class="u_pointer far fa-life-ring"></i>
            <i class="u_pointer fas fa-book"></i>
            <i class="u_pointer fas fa-shopping-cart"></i>
        </div> 
    </header>
</template>

<script>
import HeaderNavBox from '../components-header/HeaderNavBox.vue'

export default {
    components: {
        HeaderNavBox,
    },
    props: {
        navList: Array,
        logoString: String,
    }
}
</script>

<style lang="scss" scoped>
    @import '../style/headerbox.scss';
    @import '../style/utility.scss';
</style>