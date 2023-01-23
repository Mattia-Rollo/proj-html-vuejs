<template>
    <div id="how-to" class="position-relative">
        <img src="./images/artist-shape-01-600x577.png" alt="">
        <img class="line" src="./images/maxcoach-shape-14-1536x343.png" alt="">
        <svg xmlns="http://www.w3.org/2000/svg" version="1.1" width="350px" height="350px" viewBox="0 0 200 202">
            <path class="fill" fill="#fef7f3"
                d="M139.374493,198.087515 C155.702187,206.99353 190.724846,197.001323 197.677982,159.049528 C204.827153,120.027728 184.496324,118.997566 188.045232,104.801934 C202.287755,83.6528313 204.827153,56.662651 190.073179,40.4146034 C153.570125,2.39058926 144.444362,48.0194062 114.025151,20.1351292 C101.727304,7.83728238 83.0989526,-6.73517414 56.2286492,3.40456297 C18.2385839,17.7404371 27.3303985,47.659333 27.3303985,69.3128542 C27.3303985,76.9370868 3.11408002,91.2696589 0.460095291,110.885776 C-2.88628833,135.619549 12.6277797,168.175291 27.3303985,179.329002 C50.6517938,205.692318 86.6478605,199.608476 102.87144,190.482713 C116.802125,182.646702 128.220783,192.003673 139.374493,198.087515 Z">
            </path>
        </svg>

        <div class="mycontainer">
            <div class="container py-5">
                <div class="py-5">
                    <div class="uptitle">Artist coaching</div>
                    <h2 class="text-center">I understand what it take to create. I can help you with</h2>
                </div>
                <div class="row flex-column flex-sm-row align-items-end py-5 text-center text-sm-start">
                    <CardComp :array="listCards" :path="'./images/artist-box-image-'" :typeImage="'.png'" />
                </div>
                <div id="" class="row py-5 justify-content-between">
                    <div class="col-md-6 col-12 position-relative">
                        <div id="quote" class="text-center"><img src="./images/artist-quote-icon.png" alt=""
                                class="img-fluid">
                        </div>
                        <div class="fw-bold display-6 text-center px-5">I coach and mentor visual artists, like you, to
                            Create Like You Mean it</div>
                        <div class="uptitle py-4 fs-1">Martin Garrix</div>
                    </div>
                    <div class="col-md-6 col-12">
                        <p>As a coach and mentor, my ultimate goal is to motivate visual artists toward inspired action.
                            iHelp you get you back on track to being the productive, creative, meaningful and authentic
                            artist you truly want to be. i support artists in crafting and living a creative life as
                            well as felling good about themselves and their art</p>
                        <p>As an artist and an educator fro nearly 30 years, I understand what it takes to create.</p>
                        <button class="btn">get started today</button>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import CardComp from './Cards/CardComp.vue';

export default {
    name: "HowToCoachComp",
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
    components: { CardComp }
}
</script>

<style lang="scss" scoped>
#how-to {
    overflow: hidden;

    &>img {
        position: absolute;
    }

    h2 {
        max-width: 520px;
        margin: 0 auto;
        padding: 0.7rem 0 0 0;
    }

    &>img:first-child {
        top: 50px;
        left: -100px;
        z-index: 100;
        transform: rotate(-90deg);
    }

    img.line {
        top: 100px;
        z-index: -1;
        width: 100%;

    }

    svg {
        position: absolute;
        right: 100px;
        top: 400px;
        z-index: -1;
    }

    button {
        padding: 0.5rem 1.2rem;
    }
}

#quote {
    position: absolute;
    left: 50%;
    top: -15%;
}

.mycontainer {
    max-width: 1100px;
}
</style>