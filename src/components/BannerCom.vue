<template>
    <div class=" text-center banner ">
        <span>start TOMORROW! Our biggest event of the year... </span>
        <span><i class="fa-regular fa-clock"></i><span>{{ getTime() }}</span></span>
        <button class="btn"> Get Ticket</button>
    </div>
</template>

<script>
export default {
    name: 'BannerComp',
    data() {
        return {
            time: new Date('0')
        }
    },
    methods: {
        getTime() {
            this.time.setHours(0, 0, 0, 0);
            // console.log(this.time)
            return this.time.toLocaleTimeString();
        }
    },
}
</script>

<style lang="scss" scoped>
@use '../assets/style/partials/variables' as *;

.banner {
    background-color: $silver;
    // line-height: 1.5rem;
    padding: 0.6rem 0;

    span {
        display: inline-block;
        padding: 0 .5rem;

        i {
            padding: 0 0.5rem;
        }

        span {
            padding: 0;
            font-weight: 700;
        }
    }
}
</style>