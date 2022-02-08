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
    @import url('https://use.fontawesome.com/releases/v5.7.1/css/all.css');

    nav {
        display: flex;
        justify-content: space-between;
        align-items: center;

        .right-side {
            display: flex;

            ul {
                display: flex;
            }
        }
    }
</style>