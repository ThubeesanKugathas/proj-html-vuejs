<template>
    <div class="component">
        <div class="container">
            <div class="text">
                <p>WANNA TRASFORM YOUR LIFE?</p>
                <h2>Glad to Help You Learn</h2>
            </div>
            <div class="help-container">
                <div class="help">
                    <i class="far fa-flag"></i>
                    <h3>Idea Discussion</h3>
                    <p>
                        Get teamed up with the specialists who work and teach coding for years at famous universities.
                    </p>
                </div>
                <div class="help">
                    <i class="far fa-flag"></i>
                    <h3>Idea Discussion</h3>
                    <p>
                        Get teamed up with the specialists who work and teach coding for years at famous universities.
                    </p>
                </div>
                <div class="help">
                    <i class="far fa-flag"></i>
                    <h3>Idea Discussion</h3>
                    <p>
                        Get teamed up with the specialists who work and teach coding for years at famous universities.
                    </p>
                </div>
                <div class="help">
                    <i class="far fa-flag"></i>
                    <h3>Idea Discussion</h3>
                    <p>
                        Get teamed up with the specialists who work and teach coding for years at famous universities.
                    </p>
                </div>
            </div>
            <img src="../assets/home-6-services-image-1024x411.png" alt="home services image">
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
        background: rgb(238,238,238);
        background: linear-gradient(0deg, rgba(238,238,238,1) 0%, rgba(255,255,255,1) 100%);
        padding: 50px;

        .container {
            width: $c-width;
            margin: 0 auto;

            .text {
                text-align: center;
                margin-bottom: 20px;
            }

            .help-container {
                display: flex;
                justify-content: space-between;

                .help {
                    width: calc((100% - 80px) / 4);
                    margin: 10px 0;
                }
            }

            img {
                width: 100%;
                margin-top: 50px;
            }
        }
    }
</style>