<template>
    <footer>
        <div class="container">
            <ul>
                <li>ADDRESS
                    <ul>
                        <li>{{street}}</li>
                        <li>{{number}}</li>
                        <li>{{email}}</li>
                        <li>
                            <i class="fab fa-facebook-square"></i>
                            <i class="fab fa-twitter"></i>
                            <i class="fab fa-instagram"></i>
                            <i class="fab fa-linkedin"></i>
                        </li>
                    </ul>
                </li>
            </ul>
            <div class="right-side">
                <ul>
                    <li>EXPLORE
                        <ul class="explore">
                            <li v-for="(link, index) in exploreLinks" :key="index">{{link}}</li>
                        </ul>
                    </li>
                    <li>INFORMATION
                        <ul>
                            <li v-for="(link, index) in informationLinks" :key="index">{{link}}</li>
                        </ul>
                    </li>
                </ul>
            </div>
        </div>
        <p>
            <i class="far fa-copyright"></i>
            2020 Maxcoach.All Rights Reserved
        </p>
        <div class="freccia">freccia</div>
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
</style>