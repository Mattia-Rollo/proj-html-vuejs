<template>
  <BannerCom />
  <header>
    <HeaderComponent />
  </header>
  <JumbotronComp />
  <HowToCoachComp />
</template>

<script>
import BannerCom from './components/BannerCom.vue';
import HeaderComponent from './components/HeaderComponent.vue';
import HowToCoachComp from './components/HowToCoachComp.vue';
import JumbotronComp from './components/JumbotronComp.vue';

export default {
  components: { HeaderComponent, BannerCom, JumbotronComp, HowToCoachComp }
}
</script>

<style lang="scss" scoped>

</style>