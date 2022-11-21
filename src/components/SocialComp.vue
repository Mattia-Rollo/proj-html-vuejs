<template>
    <div>
        <i class="fa-brands fa-twitter"></i>
        <i class="fa-brands fa-facebook-f"></i>
        <i class="fa-brands fa-instagram"></i>
        <i class="fa-brands fa-linkedin"></i>

    </div>
</template>

<script>
export default {
    name: 'SocialComp'
}
</script>

<style lang="scss" scoped>
@use '../assets/style/partials/variables' as *;

div {
    color: gray;

    i {
        font-size: 1.5rem;
        padding: 0.8rem;
    }
}
</style>