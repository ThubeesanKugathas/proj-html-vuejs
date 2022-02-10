<template>
    <div>
        <div class="container">
            <div class="text">
                <h3>
                    Let passion and determination be the guide<br/>
                    along the way and develop at your own pace<br/>
                    that's comfortable.
                </h3>
                <p>FANNIE MORENO</p>
                <p>/Founder & CEO</p>
            </div>

            <div class="text-blocks-container">
                <!-- single stat in v-for -->
                <div v-for="(stat, i) in stats" :key="i" class="text-block">
                    <h2>{{stat.number}}</h2>
                    <p>{{stat.data}}</p>
                </div>
            </div>

            <div class="ball-container">
                <div class="ball ball-one"></div>
                <div class="ball ball-two"></div>
                <div class="ball ball-three"></div>
                <div class="ball ball-four"></div>
                <div class="ball ball-five"></div>
                <div class="ball ball-six"></div>
                <div class="ball ball-seven"></div>
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