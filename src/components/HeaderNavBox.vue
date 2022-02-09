<template>
    <nav>
        <img :src="`/navbar-logo/${logoString}.png`" alt="logo">
        <div class="right-side">
            <ul>
                <li v-for="(link, index) in navList" :key="index">{{link}}</li>
            </ul>
            <i class="fas fa-shopping-cart"></i>
            <i class="far fa-user-circle"></i>
            <input type="text" placeholder="Search">
            <i class="fas fa-search"></i>
        </div>
    </nav>
</template>

<script>
export default {
    props: {
        navList: Array,
        logoString: String,
    }
}
</script>

<style lang="scss" scoped>
    @import '../style/headernavbox.scss'
</style>