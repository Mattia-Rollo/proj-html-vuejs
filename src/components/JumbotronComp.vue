<template>
    <div class="jumbotron">
        <img src="../../public/images/artist-shape-01.png" alt="" class="w-50">
        <img src="../../public/images/artist-shape-02-768x415.png" alt="" class="w-50">
        <img src="../../public/images/artist-shape-03.png" alt="" class="puntini">
        <img src="../../public/images/artist-shape-04-127x300.png" alt="" class="w-10 piuma">
        <img src="../../public/images/artist-shape-05-300x198.png" alt="" class="">
        <div class="face"><img src="../../public/images/artist-hero-image-03.png"></div>
        <div class="pittura">
            <img src="../../public/images/artist-hero-image-02.jpg" alt="" class="img-fluid">
        </div>
        <div class="artist">
            <img src="../../public/images/artist-hero-image-04.jpg" alt="" class="img-fluid">
        </div>
        <div class="monkey">
            <img src="../../public/images/artist-hero-image-01.jpg" alt="" class="img-fluid">
        </div>
        <svg id="macchia-azzurra" xmlns="http://www.w3.org/2000/svg" version="1.1" width="350px" height="350px"
            viewBox="0 0 200 202">
            <path class="fill" fill="#b1e4f4"
                d="M139.374493,198.087515 C155.702187,206.99353 190.724846,197.001323 197.677982,159.049528 C204.827153,120.027728 184.496324,118.997566 188.045232,104.801934 C202.287755,83.6528313 204.827153,56.662651 190.073179,40.4146034 C153.570125,2.39058926 144.444362,48.0194062 114.025151,20.1351292 C101.727304,7.83728238 83.0989526,-6.73517414 56.2286492,3.40456297 C18.2385839,17.7404371 27.3303985,47.659333 27.3303985,69.3128542 C27.3303985,76.9370868 3.11408002,91.2696589 0.460095291,110.885776 C-2.88628833,135.619549 12.6277797,168.175291 27.3303985,179.329002 C50.6517938,205.692318 86.6478605,199.608476 102.87144,190.482713 C116.802125,182.646702 128.220783,192.003673 139.374493,198.087515 Z">
            </path>
        </svg>
        <svg id="macchia-gialla" xmlns="http://www.w3.org/2000/svg" version="1.1" width="200px" height="200px"
            viewBox="0 0 200 202">
            <path class="fill" fill="#efab43"
                d="M139.374493,198.087515 C155.702187,206.99353 190.724846,197.001323 197.677982,159.049528 C204.827153,120.027728 184.496324,118.997566 188.045232,104.801934 C202.287755,83.6528313 204.827153,56.662651 190.073179,40.4146034 C153.570125,2.39058926 144.444362,48.0194062 114.025151,20.1351292 C101.727304,7.83728238 83.0989526,-6.73517414 56.2286492,3.40456297 C18.2385839,17.7404371 27.3303985,47.659333 27.3303985,69.3128542 C27.3303985,76.9370868 3.11408002,91.2696589 0.460095291,110.885776 C-2.88628833,135.619549 12.6277797,168.175291 27.3303985,179.329002 C50.6517938,205.692318 86.6478605,199.608476 102.87144,190.482713 C116.802125,182.646702 128.220783,192.003673 139.374493,198.087515 Z">
            </path>
        </svg>

        <div class="hero text-center">
            <div class="uptitle">Hello, i'm Martin</div>
            <h1>Artist Coaching And Mentoring Might Be For You</h1>
            <button class="btn btn-danger">Get started today</button>
        </div>
    </div>
</template>

<script>
export default {
    name: 'JumbotronComp',
    data() {
        return {

        }
    },
}
</script>

<style lang="scss" scoped>
@use '../assets/style/partials/variables' as *;

.jumbotron {
    height: calc(100vh - 80px);
    background-color: $bg-color-jumbotron;
    position: relative;
    overflow: hidden;

    img {
        max-width: 100%;
    }

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

    .monkey {
        width: 12vw;
        bottom: 10%;
        left: 5%;
        z-index: 200;
    }

    .artist {
        width: 15vw;
        right: 8%;
        top: 30%;
        z-index: 200;
    }

    .face {
        // background-color: aqua;
        width: 10vw;
        bottom: 0;
        left: 30%;

    }

    .pittura {
        top: 10%;
        left: 15%;
        width: 12vw;
        z-index: 70;
    }

    .puntini {
        left: 30px;
        bottom: 0;
        max-width: 100%;
        z-index: 20;
    }

    .piuma {
        right: 50px;
        z-index: 40;
    }

    img[src*="shape-05"] {
        bottom: 0;
        right: 0;
    }

    svg#macchia-azzurra {
        bottom: 3px;
        left: 0;

    }

    svg#macchia-gialla {
        bottom: 25px;
        right: 185px;
        z-index: 150;

    }


    .hero {
        top: 50%;
        left: 50%;
        // height: 200px;
        max-width: 700px;
        z-index: 1000;

        transform: translate(-50%, -50%);

        .uptitle {
            font-family: 'Rosella', sans-serif;
            font-size: 3rem;
            line-height: 3rem;
            color: $cerulean;

        }

        h1 {
            // position: relative;
            padding: 1rem;
            // font-size: 3rem;

            // @media screen and (width: 500px) {
            //     font-size: 1rem;

            // }
        }

        .btn {
            display: inline-block;
            margin: 0 auto;
            padding: 0.5rem 1.2rem;
        }
    }

}
</style>