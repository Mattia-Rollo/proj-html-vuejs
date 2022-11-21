<template>
    <div class="jumbotron">
        <img src="../../public/images/artist-shape-01.png" alt="" class="w-50">
        <img src="../../public/images/artist-shape-02-768x415.png" alt="" class="w-50">
        <img src="../../public/images/artist-shape-03.png" alt="">
        <img src="../../public/images/artist-shape-04-127x300.png" alt="" class="w-10">
        <img src="../../public/images/artist-shape-05-300x198.png" alt="" class="w-10">

        <svg xmlns="http://www.w3.org/2000/svg" version="1.1" width="400px" height="400px" viewBox="0 0 200 202">
            <path class="fill" fill="#b1e4f4"
                d="M139.374493,198.087515 C155.702187,206.99353 190.724846,197.001323 197.677982,159.049528 C204.827153,120.027728 184.496324,118.997566 188.045232,104.801934 C202.287755,83.6528313 204.827153,56.662651 190.073179,40.4146034 C153.570125,2.39058926 144.444362,48.0194062 114.025151,20.1351292 C101.727304,7.83728238 83.0989526,-6.73517414 56.2286492,3.40456297 C18.2385839,17.7404371 27.3303985,47.659333 27.3303985,69.3128542 C27.3303985,76.9370868 3.11408002,91.2696589 0.460095291,110.885776 C-2.88628833,135.619549 12.6277797,168.175291 27.3303985,179.329002 C50.6517938,205.692318 86.6478605,199.608476 102.87144,190.482713 C116.802125,182.646702 128.220783,192.003673 139.374493,198.087515 Z">
            </path>
        </svg>

        <div class="hero text-center">
            <h1>Artist Coaching And Mentoring Might Be For You</h1>
            <button class="btn btn-danger">Get started today</button>
        </div>
    </div>
</template>

<script>
export default {
    name: 'JumbotronComp'
}
</script>

<style lang="scss" scoped>
@use '../assets/style/partials/variables' as *;

.jumbotron {
    height: 100vh;
    background-color: $bg-color-jumbotron;
    position: relative;
    overflow: hidden;

    &>* {
        position: absolute;
    }

    img[src*="-shape-01"] {
        width: 200px;
        right: 30px;
        z-index: 30;
    }

    img[src*="-shape-02"] {
        // width: 200px;
        z-index: 10;
    }

    img[src*="-shape-03"] {
        left: 30px;
        bottom: 0;
        max-width: 100%;
        z-index: 20;
    }

    img[src*="-shape-04"] {
        bottom: 0;
        z-index: 40;
    }

    img[src*="shape-05"] {
        bottom: 0;
        right: 0;
    }

    svg {

        bottom: 3px;
        left: 0;

    }

    .hero {
        top: 50%;
        left: 50%;
        height: 200px;

        transform: translate(-50%, -50%);

        h1 {
            // position: relative;
            padding: 1rem;
        }

        .btn {
            display: inline-block;
            margin: 0 auto;
            padding: 0.5rem 1.2rem;
        }
    }

}
</style>