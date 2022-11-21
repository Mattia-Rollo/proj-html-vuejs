<template>
    <div class="container d-flex justify-content-between">
        <div class="logo">
            <img src="/images/dark-logo.png" alt="">
        </div>
        <NavbarComp />
        <div>

        </div>
        <SocialComp />
    </div>
</template>

<script>
import NavbarComp from './NavbarComp.vue';
import SocialComp from './SocialComp.vue';

export default {
    nam: "HeaderComponent",
    components: { NavbarComp, SocialComp }
}
</script>

<style lang="scss" scoped>
div.container {
    padding: 1rem 0;
}
</style>