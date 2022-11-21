<template>
    <div class="wrapper">
        <div class="container">
            <div class="uptitle">Testimonials</div>
            <h2 class="text-center">Why do people love me?</h2>
            <div class="box"></div>
            <div class="row">
                cards
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Testimonals',
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
                    title: 'High leve of efficency and scientific teaching methods',
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
                {
                    title: 'Professional team of specialists and passionate mentors at reach',
                    comment: 'I need to get a certification for English proficiency and MaxCoach is my best choice. Their tutors are smart and professional when dealing with students.',
                    avatarImg: '04',
                    name: 'Madley Pondor',
                    job: '/IT Specialist',

                },
            ]
        }
    },
}
</script>

<style lang="scss" scoped>
@use '../assets/style/partials/variables' as *;

.wrapper {
    padding: 1rem 0;
    background-color: $beige-bg;

    .box {
        height: 300px;
    }
}
</style>