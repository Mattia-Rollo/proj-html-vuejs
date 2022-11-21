<template>
    <ul class="d-flex justify-content-between">
        <li v-for="(item, index) in menu" :key="index">{{ item }} <i class="fa-solid fa-angle-down"></i></li>
    </ul>
</template>

<script>
export default {
    name: 'NavbarComp',
    props: ['menu']

}
</script>

<style lang="scss" scoped>
@use '../assets/style/partials/variables' as *;

ul {
    list-style: none;
    margin: 0;
    padding: 0;

    li {
        height: 100%;
        padding: 0 0.8rem;


    }
}
</style>