<template>
    <main>
        <main-part-one />
        <main-part-two />
        <main-part-three />
        <main-part-four />
    </main>
</template>

<script>
import MainPartOne from './MainPartOne.vue'
import MainPartTwo from './MainPartTwo.vue'
import MainPartThree from './MainPartThree.vue'
import MainPartFour from './MainPartFour.vue'

export default {
    components: {
        MainPartOne,
        MainPartTwo,
        MainPartThree,
        MainPartFour,
    }
}
</script>

<style lang="scss" scoped>

</style>