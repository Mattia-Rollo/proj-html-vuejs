<template>
    <div class="wrapper">
        <img src="/images/artist-shape-01-300x288.png" alt="">
        <img class="right-shape" src="/images/artist-shape-01-300x288.png" alt="">
        <div class="text-side d-none d-lg-block">Courses</div>
        <div class="container">
            <div class="uptitle">
                Artist Coaching
            </div>
            <h2 class="text-center pb-5">Lastest Online Courses</h2>
            <div class="row   g-2">
                <CardComp :array="listCourses" :path="'/images/artist-course-'" :typeImage="'-480x480.jpg'" />
            </div>
        </div>
        <div class="text-center py-5">
            <button class="btn btn-danger fs-4">View All Courses <i class="fa-solid fa-arrow-right"></i></button>
        </div>

    </div>
</template>

<script>
import CardComp from './Cards/CardComp.vue'
export default {
    name: 'NewCourses',
    components: { CardComp },
    data() {
        return {
            listCourses: [
                {
                    image: '01',
                    title: 'The Acrylic Painting Accademy',
                    price: '$18.00',
                    lessons: '4',
                    students: '50',
                },
                {
                    image: '02',
                    title: 'Drawing and Shading: Complete Course',
                    price: '$21.00',
                    lessons: '14',
                    students: '50',
                },
                {
                    image: '03',
                    title: 'The Color Theory for Digital Artist',
                    price: '$19.00',
                    lessons: '7',
                    students: '50',
                },
                {
                    image: '05',
                    title: 'Ultimate Guide to Digital Sketching for Beginner',
                    price: '$35.00',
                    lessons: '14',
                    students: '50',
                },
                {
                    image: '04',
                    title: 'Portrait Drawing The Smart Way',
                    price: '$19.00',
                    lessons: '2',
                    students: '50',
                },
                {
                    image: '06',
                    title: 'Mastering Watercolor Painting from Beginner',
                    price: '$19.00',
                    lessons: '9',
                    students: '50',
                },
                {
                    image: '07',
                    title: 'The Art & Science of Drawng',
                    price: '$25.00',
                    lessons: '4',
                    students: '50',
                },
                {
                    image: '08',
                    title: 'The Colored Pencil Drawing Course',
                    price: '$21.00',
                    lessons: '6',
                    students: '50',
                },
            ]
        }
    },
}
</script>

<style lang="scss" scoped>
@use '../assets/style/partials/variables' as *;

.wrapper {
    padding: 50px 0;
    position: relative;
    overflow: hidden;

    &>img {
        position: absolute;

        &:first-child {
            left: -50px;
            top: 200px;
            filter: hue-rotate(240deg);
            z-index: -100;
        }

    }

    .right-shape {
        top: 30%;
        // background-color: rgb(255, 0, 0);
        right: 0;
        width: 300px;
        transform: rotate(-90deg);
        z-index: -100;
    }




    div.text-side {
        position: absolute;
        color: rgba($color: #000000, $alpha: 0);
        right: -230px;
        font-size: 9.5rem;
        display: inline-block;
        font-weight: 700;
        top: 50%;
        z-index: -100;
        // text-transform: uppercase;
        transform: rotate(90deg);
        -webkit-text-stroke: 1px $primary-color;
    }
}

.btn {
    vertical-align: middle;
}
</style>