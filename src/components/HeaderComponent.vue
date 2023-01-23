<template>
    <div class="container d-flex justify-content-between align-items-center">
        <div class="logo">
            <img src="./images/dark-logo.png" alt="">
        </div>
        <nav class="d-none d-md-block">
            <NavbarComp :menu="MenuNav" />
        </nav>
        <div class="d-block d-md-none fs-3"><i class="fa-solid fa-bars"></i></div>
        <SocialComp />
    </div>
</template>

<script>
import NavbarComp from './HeaderChild/NavbarComp.vue';
import SocialComp from './HeaderChild/SocialComp.vue';

export default {
    nam: "HeaderComponent",
    components: { NavbarComp, SocialComp },
    data() {
        return {
            MenuNav: ['Home', 'Pages', 'Courses', 'Features', 'Blog', 'Shop']
        }
    },
}
</script>

<style lang="scss" scoped>
div.container {
    padding: 1rem 0;

    div.logo {
        img {
            height: 30px;
        }
    }
}
</style>