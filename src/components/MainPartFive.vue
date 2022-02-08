<template>
    <div class="component">
        <div class="container">
            <div class="text">
                <p> ENJOY READING ON MAXCOACH</p>
                <h2>Latest on Our Blogs</h2>
            </div>
            <div class="blogs-container">
                <div class="blog">
                    <img src="../assets/artist-blog-01-480x325.jpeg" alt="artist blog 01">
                    <p>ARTIST</p>
                    <h3>Brush Stroke Energize Trees in Paiting</h3>
                    <i class="far fa-calendar"></i>
                    <span>May 15, 2020</span>
                    <i class="far fa-eye"></i>
                    <span>688 views</span>
                </div>
                <div class="blog">
                    <img src="../assets/artist-blog-01-480x325.jpeg" alt="artist blog 01">
                    <p>ARTIST</p>
                    <h3>Brush Stroke Energize Trees in Paiting</h3>
                    <i class="far fa-calendar"></i>
                    <span>May 15, 2020</span>
                    <i class="far fa-eye"></i>
                    <span>688 views</span>
                </div>
                <div class="blog">
                    <img src="../assets/artist-blog-01-480x325.jpeg" alt="artist blog 01">
                    <p>ARTIST</p>
                    <h3>Brush Stroke Energize Trees in Paiting</h3>
                    <i class="far fa-calendar"></i>
                    <span>May 15, 2020</span>
                    <i class="far fa-eye"></i>
                    <span>688 views</span>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
    @import '../style/variables.scss';

    .component {
        background-color: #f8f8f8;
        padding: 50px;

        .container {
            width: $c-width;
            margin: 0 auto;

            .text {
                text-align: center;
                margin-bottom: 20px;
            }

            .blogs-container {
                display: flex;
                justify-content: space-between;

                .blog {
                    width: calc((100% - 60px) / 3);
                    margin: 10px 0;

                    img {
                        max-width: 100%;
                    }
                }
            }

        }
    }
</style>