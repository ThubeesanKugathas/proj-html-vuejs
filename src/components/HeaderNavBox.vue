<template>
    <nav>
        <img :src="`/navbar-logo/${logoString}.png`" alt="logo">
        <div class="right-side">
            <ul>
                <li v-for="(link, index) in navList" :key="index">
                    {{link}}
                    <i class="fas fa-angle-down"></i>
                </li>
            </ul>
            <i class="fas fa-shopping-cart">
                <div class="cart-items">0</div>
            </i>
            <i class="far fa-user-circle"></i>
            <div class="input">
                <input type="text" placeholder="Search">
                <i class="fas fa-search"></i>
            </div>
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