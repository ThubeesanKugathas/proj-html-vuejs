<template>
    <div class="component">
        <div class="u_container">
            <h2 class="u_text-centered">Why People Talk About <span>MaxCoach</span>?</h2>

            <!-- main review -->
            <div class="u_d-flex u_justify-center u_align-items-center review">
                <!-- avatar decoration with position -->
                <div class="u_position-relative img-box">
                    <div id="brown-dot" class="u_position-absolute u_radius-50"></div>
                    <img id="avatar" class="u_position-absolute u_radius-50" src="../assets/testimonial-avata-02.jpg" alt="testimonial avatar">
                    <img id="green-dots" class="u_position-absolute" src="../assets/maxcoach-shape-05-100x100.png" alt="shape 05">
                </div>
                <!-- text review -->
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
            <div class="u_d-flex u_justify-center sponsor-container">
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