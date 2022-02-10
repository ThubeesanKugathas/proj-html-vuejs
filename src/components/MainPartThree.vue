<template>
    <div class="component">
        <div class="container">
            <div class="text">
                <p>CHOOSE A COURSE TO GET STARTED</p>
                <h2>Latest Featured <span>Courses</span></h2>
            </div>
            <!-- single course in v-for -->
            <div class="course-container">
                <div v-for="(course, i) in courses" :key="i" class="course">
                    <div class="image" :style="{ backgroundImage: `url(/maincourses/${course.course_image})`}"></div>
                    <div class="right-side">
                        <p>{{course.price}}</p>
                        <p>{{course.course_name}}</p>
                        <i class="far fa-file-alt"></i>
                        <span>{{course.lessons}} Lessons</span>
                        <i class="fas fa-user-alt"></i>
                        <span>{{course.students}} Students</span>
                    </div>
                </div>
            </div>
            <div class="button-text">
                <div class="button">
                    View all courses
                    <i class="fas fa-arrow-right"></i>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    props: {
        courses: Array,
    }
}
</script>

<style lang="scss" scoped>
    @import '../style/main/mainpartthree.scss';
    @import '../style/utility.scss';
</style>