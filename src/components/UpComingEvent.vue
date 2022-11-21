<template>

    <div class="wrapper">
        <div class="mycontainer">
            <div class="container-lg py-5">
                <div class="pb-5">
                    <div class="uptitle pb-2">
                        Up Coming Events
                    </div>
                    <h2 class="text-center pb-5">Lest's Work Together</h2>
                </div>
                <div class="row g-3">
                    <div class="col-6" v-for="(item, index) in listEvents" :key="index">
                        <div class="mycard d-flex">
                            <div v-if="index < 2">
                                <img :src="`/images/artist-event-${item.path_img}-250x300.jpg`" alt="" class="h-100">
                            </div>
                            <div class="p-4 d-flex flex-column justify-content-center"
                                :class="{ 'text-end': index >= 2 }">
                                <div class="text-secondary py-2">{{ item.date }}</div>
                                <h4>{{ item.event }}</h4>
                                <div class="text-secondary"><i class="fa-solid fa-location-dot px-1"></i>{{
                                        item.location
                                }}
                                </div>
                            </div>
                            <div v-if="index >= 2">
                                <img :src="`/images/artist-event-${item.path_img}-250x300.jpg`" alt="" class="h-100">
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'UpComingEvent',
    data() {
        return {
            listEvents: [
                {
                    path_img: '04',
                    date: 'NOV 22, 2020',
                    event: 'Storytelling Workshop',
                    location: 'Texas, US'
                },
                {
                    path_img: '03',
                    date: 'OCT 10, 2020',
                    event: 'Painting Art Contest 2020',
                    location: 'New York, US'
                },
                {
                    path_img: '02',
                    date: 'NOV 23, 2020',
                    event: 'International Art Fair 2020',
                    location: 'Hamburg, Germany'
                },
                {
                    path_img: '01',
                    date: 'DEC 15, 2020',
                    event: 'Street Performance: Call for Artist',
                    location: 'Illinois, US'
                },
            ]
        }
    },
}
</script>

<style lang="scss" scoped>
.mycard {
    height: 200px;
}
</style>