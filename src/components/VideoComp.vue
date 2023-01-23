<template>
    <div class="wrapper">
        <div class="onda">
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320">
                <path fill="#fef7f3" fill-opacity="1"
                    d="M0,192L34.3,208C68.6,224,137,256,206,250.7C274.3,245,343,203,411,176C480,149,549,139,617,165.3C685.7,192,754,256,823,266.7C891.4,277,960,235,1029,197.3C1097.1,160,1166,128,1234,122.7C1302.9,117,1371,139,1406,149.3L1440,160L1440,320L1405.7,320C1371.4,320,1303,320,1234,320C1165.7,320,1097,320,1029,320C960,320,891,320,823,320C754.3,320,686,320,617,320C548.6,320,480,320,411,320C342.9,320,274,320,206,320C137.1,320,69,320,34,320L0,320Z">
                </path>
            </svg>
        </div>

        <img id="shape" src="./images/maxcoach-shape-12-150x150.png" alt="">
        <svg xmlns="http://www.w3.org/2000/svg" version="1.1" width="250px" height="250px" viewBox="0 0 200 202">
            <path class="fill" fill="#b1e4f4"
                d="M139.374493,198.087515 C155.702187,206.99353 190.724846,197.001323 197.677982,159.049528 C204.827153,120.027728 184.496324,118.997566 188.045232,104.801934 C202.287755,83.6528313 204.827153,56.662651 190.073179,40.4146034 C153.570125,2.39058926 144.444362,48.0194062 114.025151,20.1351292 C101.727304,7.83728238 83.0989526,-6.73517414 56.2286492,3.40456297 C18.2385839,17.7404371 27.3303985,47.659333 27.3303985,69.3128542 C27.3303985,76.9370868 3.11408002,91.2696589 0.460095291,110.885776 C-2.88628833,135.619549 12.6277797,168.175291 27.3303985,179.329002 C50.6517938,205.692318 86.6478605,199.608476 102.87144,190.482713 C116.802125,182.646702 128.220783,192.003673 139.374493,198.087515 Z">
            </path>
        </svg>
        <div class="video">
            <a href="" class="link-youtube"><img src="/images/icon-youtube-play.png" alt=""></a>
            <img src="/images/artist-video-poster.jpg" alt="" class="img-fluid">

        </div>
    </div>
</template>

<script>
export default {
    name: 'VideoComp'
}
</script>

<style lang="scss" scoped>
@use '../assets/style/partials/variables' as *;

.wrapper {
    position: relative;
    padding: 5rem 0;

    // background-color: blueviolet;
    // background-image: url('/images/wave.svg');


    // background-repeat: no-repeat no-repeat;
    // transform: rotate(180deg);
    // background-size: cover;
    // background-size: 1200px;
    // background-position: center;
    .onda {
        position: absolute;
        bottom: 0;
        width: 100%;
        // background-color: $bayofmany;

        svg {
            position: relative;
            // width: 100%;
        }

    }

    #shape {
        position: absolute;
        top: 50px;
        left: 250px;
        z-index: -1;
    }

    &>svg {
        position: absolute;
        top: -10px;
        left: 200px;
        z-index: -2;
    }

}

.video {
    background-color: aqua;
    display: table;
    margin: 0 auto;
    position: relative;
    overflow: hidden;

    a {
        display: flex;
        position: absolute;
        width: 100%;
        height: 100%;
        transition: all 1s;

        img {
            margin: auto;
            z-index: 100;

        }
    }



    img {
        display: inline-block;
        margin: 0 auto;
        transition: transform 1s;

    }

    a:hover~img {
        transform: scale(1.2);
        z-index: -100;
    }

    img:last-child:hover {
        transform: scale(1.2);
    }



}
</style>