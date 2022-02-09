<template>
    <main>
        <main-part-one :stats="stats"/>
        <main-part-two />
        <main-part-three :courses="courses"/>
        <main-part-four :sponsors="sponsors"/>
        <main-part-five :blogs="blogs"/>
        <main-part-six />
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