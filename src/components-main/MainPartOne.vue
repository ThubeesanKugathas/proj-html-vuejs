<template>
    <div>
        <div class="u_container u_text-centered u_position-relative container">
            <div class="text">
                <h3>
                    Let passion and determination be the guide<br/>
                    along the way and develop at your own pace<br/>
                    that's comfortable.
                </h3>
                <p>FANNIE MORENO</p>
                <p>/Founder & CEO</p>
            </div>
        
            <div class="u_d-flex u_justify-between text-blocks-container">
                <!-- single stat in v-for -->
                <div class="text-block" v-for="(stat, i) in stats" :key="i">
                    <h2>{{stat.number}}</h2>
                    <p>{{stat.data}}</p>
                </div>
            </div>

            <!-- colored balls decoration -->
            <div class="u_container u_position-relative u_position-absolute ball-container">
                <div class="u_radius-50 u_position-absolute ball-one"></div>
                <div class="u_radius-50 u_position-absolute ball-two"></div>
                <div class="u_radius-50 u_position-absolute ball-three"></div>
                <div class="u_radius-50 u_position-absolute ball-four"></div>
                <div class="u_radius-50 u_position-absolute ball-five"></div>
                <div class="u_radius-50 u_position-absolute ball-six"></div>
                <div class="u_radius-50 u_position-absolute ball-seven"></div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    props: {
        stats: Array,
    }
}
</script>

<style lang="scss" scoped>
    @import '../style/main/mainpartone.scss';
    @import '../style/utility.scss';
</style>