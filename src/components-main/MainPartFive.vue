<template>
    <div class="component">
        <div class="u_container">
            <div class="u_text-centered text">
                <p> ENJOY READING ON MAXCOACH</p>
                <h2>Latest on <span>Our Blogs</span></h2>
            </div>
            <!-- single blog in v-for -->
            <div class="u_d-flex u_justify-between">
                <div v-for="(blog, i) in blogs" :key="i" class="blog">
                    <img :src="`/mainblog/${blog.thumbnail}`" :alt="blog.thumbnail">
                    <p>{{blog.author}}</p>
                    <h3>{{blog.title}}</h3>
                    <i class="far fa-calendar"></i>
                    <span>{{blog.date}}</span>
                    <i class="far fa-eye"></i>
                    <span>{{blog.views}} views</span>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    props: {
        blogs: Array,
    }
}
</script>

<style lang="scss" scoped>
    @import '../style/main/mainpartfive.scss';
    @import '../style/utility.scss';
</style>