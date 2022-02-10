<template>
    <div class="component">
        <div class="container">
            <!-- final raccomandation -->
            <div class="text">
                <p>Start today for getting <span>Online Certification</span></p>
                <h2>You can be your own guiding star with our help!</h2>
                <div class="button">Get started now</div>
            </div>
            
            <div class="ball-container-two">
                <div class="ball ball-one"></div>
                <div class="ball ball-two"></div>
                <div class="ball ball-three"></div>
                <div class="ball ball-four"></div>
                <div class="ball ball-five"></div>
                <div class="ball ball-six"></div>
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
                cursor: pointer;

                &:hover {
                    background-color: #1f2154;
                }
            }
        }

        .ball-container-two {
            height: 600px;
            position: relative;
            width: $c-width;
            margin: 0 auto;
            position: absolute;
            top: 450%;
        
            .ball {
                border-radius: 50%;
                position: absolute;
            }
        
            .ball-one {
                width: 30px;
                height: 30px;
                border: 5px solid $green;
                top: 40%;
                left: 60px;
            }
        
            .ball-two {
                width: 25px;
                height: 25px;
                background-color: #cc1b17;
                bottom: -70px;
                left: -300px;
            }
        
            .ball-three {
                width: 40px;
                height: 40px;
                background-color: #febc4d;
                bottom: -300px;
                left: -250px;
            }
        
            .ball-four {
                width: 30px;
                height: 30px;
                background-color: $green;
                right: 0;
                top: 50%;
            }
        
            .ball-five {
                width: 25px;
                height: 25px;
                background-color: #e25a6d;
                right: 100px;
                bottom: -150px;
            }
        
            .ball-six {
                width: 25px;
                height: 25px;
                background-color: #866deb;
                right: -200px;
                bottom: -300px;
            }
        }
    }
</style>