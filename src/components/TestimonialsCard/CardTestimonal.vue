<template>
    <div class="col h-100" v-for="(item, index) in  array" :key="index">
        <div class="myCard" :class="index == activeIndex ? 'active' : ''">
            <h4 class="py-2">{{ item.title }}</h4>
            <p>{{ item.comment }}</p>
            <div class="d-flex gap-3">
                <div class="avatar"><img :src="`./images/artist-testimonial-avatar-${item.avatarImg}.jpg`" alt=""
                        class="img-fluid"> </div>
                <div class="d-flex flex-column  justify-content-evenly">
                    <strong>{{ item.name }}</strong>
                    <div>{{ item.job }}</div>
                </div>
            </div>
        </div>
    </div>

</template>

<script>
export default {
    name: 'CardTestimonial',
    props: {
        array: Array
    },
    data() {
        return {
            activeIndex: 1
        }
    },
}
</script>

<style lang="scss" scoped>
@use '../../assets/style/partials/variables' as *;

.avatar {
    width: 80px;
    border-radius: 50%;
    overflow: hidden;
}

.myCard {
    width: 450px;
    padding: 1.5rem;
    background-color: white;
    border-radius: 10px;
    opacity: 0.6;
    margin: 0 0.5rem;

}

.active {
    opacity: 1;
    // transform: scale(1.2);
    // transform: translatex(-50px, 0);
    z-index: 200;
    border: 1px solid $light;
}
</style>