<template>
    <main>
        <!-- stats data -->
        <main-part-one :stats="stats"/>
        <!-- main information -->
        <main-part-two />
        <!-- latest courses -->
        <main-part-three :courses="courses"/>
        <!-- reviews and sponsor/clients -->
        <main-part-four :sponsors="sponsors"/>
        <!-- blogs from artists -->
        <main-part-five :blogs="blogs"/>
        <!-- help new infos -->
        <main-part-six :infos="helpInfos"/>
        <!-- last advice + button -->
        <main-part-seven />
    </main>
</template>

<script>
import MainPartOne from '../components-main/MainPartOne.vue'
import MainPartTwo from '../components-main/MainPartTwo.vue'
import MainPartThree from '../components-main/MainPartThree.vue'
import MainPartFour from '../components-main/MainPartFour.vue'
import MainPartFive from '../components-main/MainPartFive.vue'
import MainPartSix from '../components-main/MainPartSix.vue'
import MainPartSeven from '../components-main/MainPartSeven.vue'

export default {
    components: {
        MainPartOne,
        MainPartTwo,
        MainPartThree,
        MainPartFour,
        MainPartFive,
        MainPartSix,
        MainPartSeven,
    },
    props: {
        stats: Array,
        blogs: Array,
        courses: Array,
        sponsors: Array,
        helpInfos: Array,
    }
}
</script>

<style lang="scss" scoped>

</style>