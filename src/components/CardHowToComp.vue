<template>
    <div class="col" v-for="(item, index) in array" :key="index">
        <div class="mycard">
            <img :src="`/public/images/artist-box-image-${item.image}.png`" :alt="item.alt" class="img-fluid">
            <h4>{{ item.title }}</h4>
            <p>{{ item.overview }}</p>
        </div>
    </div>
</template>

<script>
export default {
    name: 'CardHowToComp',
    props: {
        array: Array
    }
}
</script>

<style lang="scss" scoped>
.mycard {
    height: 100%;

}
</style>