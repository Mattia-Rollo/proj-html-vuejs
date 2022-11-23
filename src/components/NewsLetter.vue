<template>
    <div class="wrapper d-flex">
        <img class="d-none d-md-block" src="/images/artist-shape-color-paint-top-left.png" alt="">


        <div class="container-lg ">
            <div class="row align-items-center text-light h-100">
                <div class="col-12 col-md-4">
                    <h3 class=" text-end w-75">NewsLetter to get in Touch</h3>
                </div>
                <div class="col-12 col-md-8 ">
                    <a href="">
                        <div id="email" class="border-bottom border-1 fs-4 d-flex justify-content-between">Your
                            Email <i class="fa-solid fa-arrow-right"></i></div>
                    </a>
                </div>
            </div>
        </div>

        <img class="d-none d-md-block" src="/images/artist-shape-color-paint-bottom-right.png" alt="">
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
        position: relative;
        height: 100%;
    }

    img:first-child {
        left: 0;
    }

    img:nth-child(2) {
        right: 0;

    }

    a {
        text-decoration: none;
        color: $white;
    }
}
</style>