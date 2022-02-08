<template>
    <header>
        <!-- IMG BACKGROUND SVG's -->
        <!-- <img src="../assets/jumbotron-background-wave-small.svg" alt="small wave">
        <img src="../assets/jumbotron-background-wave-medium.svg" alt="medium wave">
        <img src="../assets/jumbotron-background-wave-big.svg" alt="big wave"> -->
        <div class="container">
            <!-- navbar component -->
            <header-nav-box :navList="navList" :logoString="logoString"/>
            <!-- central title + button -->
            <div class="header-title">
                <h2>Learn At Your Own Pace!</h2>
                <p>Get teamed up with people of same will</p>
                <div class="header-button">Get started for free</div>
            </div>
            <!-- 3 img  -->
            <div class="header-images">
                <img src="../assets/home-6-hero-left-person.png" alt="left-person">
                <!-- center image da posizionare centralmente tramite position, così da coprire leggermente hero-left -->
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