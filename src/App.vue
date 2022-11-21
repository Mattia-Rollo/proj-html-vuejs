<template>
  <BannerCom />
  <header>
    <HeaderComponent />
  </header>
  <JumbotronComp />
  <HowToCoachComp />
  <VideoComp />
  <Testimonials />
</template>

<script>
import BannerCom from './components/BannerCom.vue';
import HeaderComponent from './components/HeaderComponent.vue';
import HowToCoachComp from './components/HowToCoachComp.vue';
import JumbotronComp from './components/JumbotronComp.vue';
import Testimonials from './components/Testimonials.vue';
import VideoComp from './components/VideoComp.vue';

export default {
  components: { HeaderComponent, BannerCom, JumbotronComp, HowToCoachComp, VideoComp, Testimonials }
}
</script>

<style lang="scss" scoped>

</style>