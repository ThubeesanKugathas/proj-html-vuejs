<template>
    <footer class="u_position-relative">
        <div class="u_container u_d-flex u_justify-between links-container">
            <ul>
                <!-- left side address section + social icons -->
                <li class="section"><strong>Address</strong>
                    <ul>
                        <li>{{street}}</li>
                        <li>{{number}}</li>
                        <li>{{email}}</li>
                        <li>
                            <a href="#/">
                                <i class="fab fa-facebook-square"></i>
                            </a>
                            <a href="#/">
                                <i class="fab fa-twitter"></i>
                            </a>
                            <a href="#/">
                                <i class="fab fa-instagram"></i>
                            </a>
                            <a href="#/">
                                <i class="fab fa-linkedin"></i>
                            </a>
                        </li>
                    </ul>
                </li>
            </ul>

            <div class="right-side">
                <ul class="u_d-flex">
                    <!-- explore section links -->
                    <li class="section"><strong>Explore</strong>
                        <ul class="u_d-flex u_wrap explore">
                            <li v-for="(link, index) in exploreLinks" :key="index">
                                <a href="#/">
                                    {{link}}
                                </a>
                            </li>
                        </ul>
                    </li>
                    <!-- information section links -->
                    <li class="section"><strong>Information</strong>
                        <ul>
                            <li v-for="(link, index) in informationLinks" :key="index">
                                <a href="#/">
                                    {{link}}
                                </a>
                            </li>
                        </ul>
                    </li>
                </ul>
            </div>
        </div>

        <!-- copyright rights text -->
        <p class="u_text-centered">
            <i class="far fa-copyright"></i>
            2020 Maxcoach.All Rights Reserved
        </p>

        <!-- button to move at the header -->
        <div class="u_position-absolute u_radius-50 freccia">
            <a href="#">
                <i class="fas fa-arrow-up"></i>
            </a>
        </div>
    </footer>
</template>

<script>
export default {
    props: {
        street: String,
        number: String,
        email: String,
        exploreLinks: Array,
        informationLinks: Array,
    }
}
</script>

<style lang="scss" scoped>
    @import '../style/footerbox.scss';
    @import '../style/utility.scss';
</style>