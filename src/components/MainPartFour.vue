<template>
    <div class="component">
        <div class="container">
            <h2>Why People Talk About <span>MaxCoach</span>?</h2>
            <!-- main review -->
            <div class="review">
                <div class="img-box">
                    <div id="brown-dot"></div>
                    <img id="avatar" src="../assets/testimonial-avata-02.jpg" alt="testimonial avatar">
                    <img id="green-dots" src="../assets/maxcoach-shape-05-100x100.png" alt="shape 05">
                </div>
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
            <!-- single sponsor in v-for -->
            <div class="sponsor-container">
                <div class="sponsor" 
                    v-for="sponsor in sponsors" 
                    :key="sponsor.name" 
                    :style="{ backgroundImage: `url(/mainsponsors/${sponsor.client_image})`}"></div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    props: {
        sponsors: Array,
    }
}
</script>

<style lang="scss" scoped>
    @import '../style/main/mainpartfour.scss';
    @import '../style/utility.scss';
</style>