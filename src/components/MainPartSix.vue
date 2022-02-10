<template>
    <div class="component">
        <div class="u_container">
            <div class="u_text-centered text">
                <p>WANNA TRASFORM YOUR LIFE?</p>
                <h2>Glad to <span>Help You</span> Learn</h2>
            </div>

            <!-- helping informations -->
            <div class="u_d-flex u_justify-between">
                <div class="help"
                    v-for="(info, i) in infos"
                    :key="i">
                    <i :class="info.icon"></i>
                    <h3>{{info.title}}</h3>
                    <p>{{info.info}}</p>
                </div>
            </div>

            <!-- image at bottom center -->
            <img src="../assets/home-6-services-image-1024x411.png" alt="home services image">
        </div>
    </div>
</template>

<script>
export default {
    props: {
        infos: Array, 
    }
}
</script>

<style lang="scss" scoped>
    @import '../style/main/mainpartsix.scss';
    @import '../style/utility.scss';
</style>