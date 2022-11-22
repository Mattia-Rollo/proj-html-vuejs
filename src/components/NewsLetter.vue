<template>
    <div class="wrapper">
        <img src="/images/artist-shape-color-paint-top-left.png" alt="">
        <img src="/images/artist-shape-color-paint-bottom-right.png" alt="">
        ciao sono newsletter
        <div class="mycontainer h-100 px-5">
            <div class="container-lg h-100">
                <div class="row align-items-center text-light">
                    <div class="col ">
                        <h3 class=" text-end w-75">NewsLetter to get in Touch</h3>
                    </div>
                    <div class="col-8 ">
                        <a href="">
                            <div id="email" class="border-bottom border-1 fs-4 d-flex justify-content-between">Your
                                Email <i class="fa-solid fa-arrow-right"></i></div>
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'NewsLetter'
}
</script>

<style lang="scss" scoped>
@use '../assets/style/partials/variables' as *;

.wrapper {
    height: 150px;
    background-color: $blue-bg-newsletter;
    position: relative;
    overflow: hidden;

    img {
        position: absolute;
    }

    img:first-child {
        left: 0;
        height: 100%;
    }

    img:nth-child(2) {
        right: 0;
        height: 100%;
    }

    a {
        text-decoration: none;
        color: $white;
    }
}
</style>