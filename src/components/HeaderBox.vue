<template>
    <header>
        <!-- IMG BACKGROUND SVG's -->
        <div class="small-box">
            <img v-for="(image, i) in 2" :key="i" class="small" src="../assets/jumbotron-background-wave-small.svg" alt="small wave">
        </div>
        <div class="medium-box">
            <img v-for="(image, i) in 2" :key="i" class="medium" src="../assets/jumbotron-background-wave-medium.svg" alt="medium wave">
        </div>
        <div class="big-box">
            <img v-for="(image, i) in 2" :key="i" class="big" src="../assets/jumbotron-background-wave-big.svg" alt="big wave">
        </div>

        <!-- container of navbar, button, title -->
        <div class="container">
            <header-nav-box :navList="navList" :logoString="logoString"/>
            <div class="header-title">
                <h2>Learn At Your Own Pace!</h2>
                <p>Get teamed up with people of same will</p>
                <div class="header-button">Get started for free</div>
            </div>
            <div class="header-images">
                <img src="../assets/home-6-hero-left-person.png" alt="left-person">
                <img id="center-image" src="../assets/video-screen.png" alt="video-screen">
                <img id="right-image" src="../assets/home-6-hero-right-person.png" alt="right-person">
            </div>
        </div> 
    </header>
</template>

<script>
import HeaderNavBox from './HeaderNavBox.vue'

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
</style>