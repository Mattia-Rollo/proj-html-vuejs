<template>
    <div class="wrapper">
        <img src="/images/artist-shape-color-paint-top-left.png" alt="">
        <img src="/images/artist-shape-color-paint-bottom-right.png" alt="">
        ciao sono newsletter
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
    height: 100px;
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
}
</style>