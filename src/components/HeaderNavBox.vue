<template>
    <nav class="u_d-flex u_justify-between u_align-items-center">
        <!-- left side logo MaxCoach interchangeable from data (app.vue) -->
        <img :src="`/navbar-logo/${logoString}.png`" alt="logo">

        <!-- right side with link and text input -->
        <div class="u_d-flex u_align-items-center right-side">
            <ul class="u_d-flex">
                <li class="u_pointer" 
                    v-for="(link, index) in navList" :key="index">
                    {{link}}
                    <i class="fas fa-angle-down"></i>
                </li>
            </ul>
            <i class="u_position-relative fas fa-shopping-cart">
                <div class="u_position-absolute u_radius-50 cart-items">0</div>
            </i>
            <i class="far fa-user-circle"></i>
            <div class="u_d-flex u_align-items-center input">
                <input type="text" placeholder="Search...">
                <i class="u_pointer fas fa-search"></i>
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
    @import '../style/headernavbox.scss';
    @import '../style/utility.scss';
</style>