<template>
    <div class="col-lg-3 col-sm-6 col-12" v-for="(item, index) in array" :key="index">
        <div class="mycard" :class="item.price ? 'moveImgEffect' : ''">
            <div class="image"><img :src="path + item.image + typeImage" :alt="item.alt" class="img-fluid"></div>

            <div :class="item.price ? 'mybody-Card' : ''">
                <div v-if="item.price" class="price">{{ item.price }}</div>
                <h5>{{ item.title }}</h5>
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
    overflow: hidden;

    .image {
        overflow: hidden;
    }


    .mybody-Card {
        padding: 1rem;
        transition: all 0.5s;
        max-width: calc(100% - 30px);
        background-color: $white;
        border: 1px solid transparent;
    }

    &:hover .mybody-Card {
        border-color: $primary-color;
        border-radius: 10px;
        transform: translateY(-30px);
    }

}


.moveImgEffect img {
    transition: all 0.5S;
}

.moveImgEffect:hover img {
    transform: scale(1.2);
}

.price {
    font-weight: 700;
    color: $thunderbird-red;
    padding: 1rem 0;
    font-size: 1.2rem;
}

.info {
    color: grey;
    font-size: 1rem;

    span {
        padding: 0 0.5rem;
    }
}
</style>