<template>
    <div>
        <a href=""><i class="fa-brands fa-twitter"></i></a>
        <a href=""><i class="fa-brands fa-facebook-f"></i></a>
        <a href=""><i class="fa-brands fa-instagram"></i></a>
        <a href=""><i class="fa-brands fa-linkedin"></i></a>

    </div>
</template>

<script>
export default {
    name: 'SocialComp',
    data() {
        return {

        }
    },
}
</script>

<style lang="scss" scoped>
@use '../assets/style/partials/variables' as *;

div {
    color: $cod-gray;

    a {
        color: $cod-gray;
        font-size: 1.5rem;
        padding: 0.5rem;
    }
}
</style>