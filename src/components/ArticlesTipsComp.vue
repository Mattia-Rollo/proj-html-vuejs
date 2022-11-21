<template>
    <div class="wrapper">
        <div class="container">
            <div class="py-5">
                <div class="uptitle">Articles and Tips</div>
                <h2 class="text-center">Latest from the blog</h2>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'ArticlesTipsComp'
}
</script>

<style lang="scss" scoped>
@use '../assets/style/partials/variables' as *;

.wrapper {
    background-color: $grey-Articles-Tips;
    height: 100vh;
}
</style>