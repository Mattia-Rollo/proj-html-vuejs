<template>
    <div class="col-lg-3 col-md" v-for="(item, index) in array" :key="index">
        <div class="mycard">
            <img :src="path + item.image + typeImage" :alt="item.alt" class="img-fluid">
            <div :class="item.price ? 'mybody-Card' : ''">
                <div v-if="item.price" class="price">{{ item.price }}</div>
                <h4>{{ item.title }}</h4>
                <p>{{ item.overview }}</p>
                <div v-if="item.lessons" class="info">
                    <span><i class="fa-regular fa-file"></i><span>{{ item.lessons }}</span> Lessons</span>
                    <span><i class="fa-regular fa-user"></i><span>{{ item.students }}</span> Students</span>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'CardComp',
    props: {
        array: Array,
        path: String,
        typeImage: String
    }
}
</script>

<style lang="scss" scoped>
@use '../../assets/style/partials/variables' as *;

.mycard {
    height: 100%;
    cursor: pointer;

    .mybody-Card {
        padding: 1rem;
        transition: all 0.5s;
        background-color: $white;
        border: 1px solid transparent;
    }

    &:hover .mybody-Card {
        border-color: $thunderbird-red;
        border-radius: 10px;
        transform: translateY(-30px);
    }

}

.price {
    font-weight: 700;
    color: $thunderbird-red;
    padding: 1rem 0;
    font-size: 1.2rem;
}

.info {
    color: grey;

    span {
        padding: 0 0.5rem;
    }
}
</style>