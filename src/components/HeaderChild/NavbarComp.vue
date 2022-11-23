<template>
    <ul class="d-flex justify-content-between gap-4">
        <li class=" overflow-hidden" v-for="(item, index) in menu" :key="index">{{ item }} <i
                class="fa-solid fa-angle-down"></i>
            <div class="border-animated"></div>
        </li>
    </ul>
</template>

<script>

export default {
    name: 'NavbarComp',
    props: {
        menu: Array
    }

}
</script>

<style lang="scss" scoped>
@use '../../assets/style/partials/variables' as *;

ul {
    list-style: none;
    margin: 0;
    padding: 0;

    li {
        height: 100%;
        // padding: 0 0.8rem;
        transition: color 0.3s ease;
        font-weight: 500;
        cursor: pointer;
        position: relative;


        &:hover {
            color: tomato;
            // border-bottom: 2px solid tomato;

        }

        .border-animated {



            width: 100%;
            height: 3px;
            // border-radius: 4px;
            background-color: black;
            bottom: 0;
            left: 0;
            transform-origin: right;
            transform: scaleX(0);
            transition: transform .3s ease-in-out, background-color .3s ease-in-out;

        }

        &:hover .border-animated {
            background-color: tomato;
            transform-origin: left;
            transform: scaleX(1);
        }


    }
}

@keyframes move {

    0% {
        transform: translatex(-100%);
    }

    100% {
        transform: translatex(100%);
    }

}
</style>