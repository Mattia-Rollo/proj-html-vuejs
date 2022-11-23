<template>
    <div class="wrapper">
        <div class="container">
            <div class="uptitle">Testimonials</div>
            <h2 class="text-center">Why do people love me?</h2>
            <!-- <div class="box"></div> -->
            <div class="d-flex ">
                <CardTestimonial :array="listTestimonials" />
            </div>
            <div class="thumb">
                <span class="dot" v-for="(item, index) in listTestimonials" :class="index == 1 ? 'active' : ''"></span>
            </div>
        </div>
    </div>
</template>

<script>
import CardTestimonial from './TestimonialsCard/CardTestimonal.vue'
export default {
    name: 'Testimonals',
    components: { CardTestimonial },
    data() {
        return {
            listTestimonials: [
                {
                    title: 'it\'s a choice of quality for people width special nedds',
                    comment: 'I\'m a very strict person so I require everything to be organized and neat. Then, I\'ll be able to make things right anc shine. MaxCoach guys just git me.',
                    avatarImg: '01',
                    name: 'Florence Themes',
                    job: '/Multimedia Admin',

                },
                {
                    title: 'High level of efficency and scientific teaching methods',
                    comment: 'I am free to learn at my own pace, follow my own schedule and choose the subject I want to learn from the syllabus. Great study portal for people like me',
                    avatarImg: '02',
                    name: 'Mina Hollance',
                    job: '/Freelancer',

                },
                {
                    title: 'Professional team of specialists and passionate mentors at reach',
                    comment: 'I need to get a certification for English proficiency and MaxCoach is my best choice. Their tutors are smart and professional when dealing with students.',
                    avatarImg: '03',
                    name: 'Madley Pondor',
                    job: '/IT Specialist',

                },
                // {
                //     title: 'The Best coaching I ever had',
                //     comment: 'With Thrive’s help, we were able to increase the functionality of our website dramatically while cutting our costs. Our website is much more easy to use, has tons of more features than before and is incredibly easy to maintain.',
                //     avatarImg: '04',
                //     name: 'Joe Satriani',
                //     job: '/CEO google',

                // },
            ]
        }
    },
}
</script>

<style lang="scss" scoped>
@use '../assets/style/partials/variables' as *;

.wrapper {
    padding: 1.5rem 0 0;
    background-color: $beige-bg;

    .box {}

    h2 {
        padding: 0 0 3rem 0;
    }
}

.thumb {
    display: table;
    margin: 0 auto;
    padding: 1rem 0;
}

.dot {
    display: inline-block;
    // margin: 1rem;
    width: 0.8rem;
    height: 0.8rem;
    border-radius: 50%;
    background-color: rgb(79, 79, 79);
    z-index: 1000;
    margin: 0 1rem;
}

.active {
    background-color: black;
}
</style>