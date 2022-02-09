<template>
    <div class="component">
        <div class="container">
            <!-- final raccomandation -->
            <div class="text">
                <p>Start today for getting <span>Online Certification</span></p>
                <h2>You can be your own guiding star with our help!</h2>
                <div class="button">Get started now</div>
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

    .container {
        width: $c-width;
        margin: 50px auto 0;
        padding: 50px;

        .text {
            text-align: center;

            p {
                font-size: 24px;
            
                span {
                    color: $green;
                }
            }

            h2 {
                font-size: 30px;
                font-weight: bold;
            }

            .button {
                background-color: $green;
                color: #fff;
                padding: 15px 40px;
                display: inline-block;
                margin-top: 30px;
                border-radius: 5px;
                font-weight: bold;
            }
        }
    }
</style>