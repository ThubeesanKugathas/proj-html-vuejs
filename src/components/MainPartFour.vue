<template>
    <div class="component">
        <div class="container">
            <h2>Why People Talk About MaxCoach?</h2>
            <div class="review">
                <img src="../assets/testimonial-avata-02.jpg" alt="testimonial avatar">
                <div class="right-side">
                    <p>
                        I am free to learn at my own pace, follow <br/>
                        my own shedule and choose the subject I <br/>
                        like. Great study portal for people like me.
                    </p>
                    <p>MINA HOLLACE</p>
                    <p>/Freelancer</p>
                </div>
            </div>
            <div class="sponsor-container">
                <div class="sponsor"></div>
                <div class="sponsor"></div>
                <div class="sponsor"></div>
                <div class="sponsor"></div>
                <div class="sponsor"></div>
                <div class="sponsor"></div>
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
        padding: 50px;

        .container {
            width: $c-width;
            margin: 0 auto;
            
            h2 {
                text-align: center;
                margin-bottom: 20px;
            }

            .review {
                display: flex;
                align-items: center;
                justify-content: center;

                .right-side {
                    margin-left: 30px;
                }
            }

            .sponsor-container {
                display: flex;
                justify-content: center;

                .sponsor {
                    width: calc(100% / 6);
                    height: 100px;
                    background-image: url('../assets/client-logo-colored-01.png');
                    background-size: contain;
                    background-repeat: no-repeat;
                    margin: 10px 10px;
                }
            }
        }
    }
</style>