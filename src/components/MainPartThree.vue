<template>
    <div class="component">
        <div class="container">
            <div class="text">
                <p>CHOOSE A COURSE TO GET STARTED</p>
                <h2>Latest Featured Courses</h2>
            </div>
            <div class="course-container">
                <div class="course">
                    <div class="image"></div>
                    <div class="right-side">
                        <p>$40.00</p>
                        <p>Learning to Write as a Professional Author</p>
                        <i class="far fa-file-alt"></i>
                        <span>20 Lessons</span>
                        <i class="fas fa-user-alt"></i>
                        <span>50 Students</span>
                    </div>
                </div>
                <div class="course">
                    <div class="image"></div>
                    <div class="right-side">
                        <p>$40.00</p>
                        <p>Learning to Write as a Professional Author</p>
                        <i class="far fa-file-alt"></i>
                        <span>20 Lessons</span>
                        <i class="fas fa-user-alt"></i>
                        <span>50 Students</span>
                    </div>
                </div>
                <div class="course">
                    <div class="image"></div>
                    <div class="right-side">
                        <p>$40.00</p>
                        <p>Learning to Write as a Professional Author</p>
                        <i class="far fa-file-alt"></i>
                        <span>20 Lessons</span>
                        <i class="fas fa-user-alt"></i>
                        <span>50 Students</span>
                    </div>
                </div>
                <div class="course">
                    <div class="image"></div>
                    <div class="right-side">
                        <p>$40.00</p>
                        <p>Learning to Write as a Professional Author</p>
                        <i class="far fa-file-alt"></i>
                        <span>20 Lessons</span>
                        <i class="fas fa-user-alt"></i>
                        <span>50 Students</span>
                    </div>
                </div>
                <div class="course">
                    <div class="image"></div>
                    <div class="right-side">
                        <p>$40.00</p>
                        <p>Learning to Write as a Professional Author</p>
                        <i class="far fa-file-alt"></i>
                        <span>20 Lessons</span>
                        <i class="fas fa-user-alt"></i>
                        <span>50 Students</span>
                    </div>
                </div>
                <div class="course">
                    <div class="image"></div>
                    <div class="right-side">
                        <p>$40.00</p>
                        <p>Learning to Write as a Professional Author</p>
                        <i class="far fa-file-alt"></i>
                        <span>20 Lessons</span>
                        <i class="fas fa-user-alt"></i>
                        <span>50 Students</span>
                    </div>
                </div>
            </div>
            <div class="button">View all courses</div>
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
        background-color: #f5f7fa;
        padding: 50px 0;

        .container {
            width: $c-width;
            margin: 0 auto;

            .text {
                text-align: center;
                margin-bottom: 50px;
            }

            .course-container {
                display: flex;
                flex-wrap: wrap;

                .course {
                    width: 50%;
                    height: 150px;
                    padding: 10px;
                    display: flex;
                    align-items: center;

                    .image {
                        height: 100%;
                        width: 130px;
                        border-radius: 50%;
                        background-image: url('../assets/course-02-480x298.jpg');
                        background-size: cover;
                        margin-right: 20px;
                    }
                }
            }

            .button {
                text-align: center;
                margin-top: 30px;
            }
        }
    }
</style>