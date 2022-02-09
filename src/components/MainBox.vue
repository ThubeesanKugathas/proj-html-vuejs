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
        <main-part-six />
        <!-- last advice + button -->
        <main-part-seven />
    </main>
</template>

<script>
import MainPartOne from './MainPartOne.vue'
import MainPartTwo from './MainPartTwo.vue'
import MainPartThree from './MainPartThree.vue'
import MainPartFour from './MainPartFour.vue'
import MainPartFive from './MainPartFive.vue'
import MainPartSix from './MainPartSix.vue'
import MainPartSeven from './MainPartSeven.vue'

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
    }
}
</script>

<style lang="scss" scoped>

</style>