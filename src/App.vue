<template>
  <BannerCom />
  <header>
    <HeaderComponent />
  </header>
  <JumbotronComp />
</template>

<script>
import BannerCom from './components/BannerCom.vue';
import HeaderComponent from './components/HeaderComponent.vue';
import JumbotronComp from './components/JumbotronComp.vue';

export default {
  components: { HeaderComponent, BannerCom, JumbotronComp }
}
</script>

<style lang="scss" scoped>

</style>