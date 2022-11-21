<template>
    <div class="position-relative">
        <img src="../../public/images/" alt="">
        <div class="container py-5">
            <div class="py-5">
                <div class="uptitle">Artist coaching</div>
                <h2 class="text-center">I understand what it take to create. I can help you with</h2>
            </div>
            <div class="row align-items-end py-5">
                <CardHowToComp :array="listCards" />
            </div>
            <div class="row py-5 justify-content-between">
                <div class="col-5 position-relative">
                    <div class="text-center"><img src="/public/images/artist-quote-icon.png" alt=""></div>
                    <div class="fw-bold display-6 text-center">Lorem ipsum dolor sit amet consectetur adipisicing elit.
                        Natus,
                        reiciendis?</div>
                    <div class="uptitle py-5">Martin Garrix</div>
                </div>
                <div class="col-6">
                    <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Quos quo fugiat quidem illum at
                        corporis?
                        Repellat perferendis placeat sed itaque odio error aut rem in maiores voluptatibus soluta,
                        sapiente
                        recusandae numquam laborum corrupti consequuntur pariatur! Ducimus natus voluptates earum
                        laudantium
                        ex at nulla eos maxime eveniet voluptate, ullam doloribus aliquam!</p>
                    <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Quaerat, delectus?</p>
                    <button class="btn btn-danger">get started today</button>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import CardHowToComp from './CardHowToComp.vue';

export default {
    name: "HowToCaochComp",
    data() {
        return {
            listCards: [
                {
                    image: '01',
                    alt: 'foglie',
                    title: 'Online Courses',
                    overview: 'Online art coaching now offers you a very powerful way to redisign your artist mind',
                },
                {
                    image: '02',
                    alt: 'arcobaleno',
                    title: 'One to One',
                    overview: 'Getting the necessary clarity about the current state to help you improve your ability',
                },
                {
                    image: '03',
                    alt: 'goccie',
                    title: 'Anywhere',
                    overview: 'Access to valuable and portable program which allow you to setup and live anywhere you want',
                },
                {
                    image: '04',
                    alt: 'eye',
                    title: 'On Time',
                    overview: 'Punctuality is our top priority because it\'s an essential criteria to access a program quality',
                },
            ]
        };
    },
    components: { CardHowToComp }
}
</script>

<style lang="scss" scoped>
img {
    position: absolute;
    top: -50px;
    z-index: 100;
}
</style>