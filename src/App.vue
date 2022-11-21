<template>
  <BannerCom />
  <header>
    <HeaderComponent />
  </header>
  <JumbotronComp />
  <HowToCoachComp />
  <VideoComp />
  <Testimonials />
  <NewCourses />
  <ArticlesTipsComp />
  <UpComingEvent />
</template>

<script>
import ArticlesTipsComp from './components/ArticlesTipsComp.vue';
import BannerCom from './components/BannerCom.vue';
import HeaderComponent from './components/HeaderComponent.vue';
import HowToCoachComp from './components/HowToCoachComp.vue';
import JumbotronComp from './components/JumbotronComp.vue';
import NewCourses from './components/NewCourses.vue';
import Testimonials from './components/Testimonials.vue';
import UpComingEvent from './components/UpComingEvent.vue';
import VideoComp from './components/VideoComp.vue';

export default {
  components: { HeaderComponent, BannerCom, JumbotronComp, HowToCoachComp, VideoComp, Testimonials, NewCourses, ArticlesTipsComp, UpComingEvent }
}
</script>

<style lang="scss" scoped>

</style>