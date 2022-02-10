<template>
    <footer>
        <div class="container">
            <ul>
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
                <ul>
                    <li class="section"><strong>Explore</strong>
                        <ul class="explore">
                            <li v-for="(link, index) in exploreLinks" :key="index">
                                <a href="#/">
                                    {{link}}
                                </a>
                            </li>
                        </ul>
                    </li>
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
        <p>
            <i class="far fa-copyright"></i>
            2020 Maxcoach.All Rights Reserved
        </p>
        <div class="freccia">
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