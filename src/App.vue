<template>
  <BannerCom />
  <header>
    <HeaderComponent />
  </header>
</template>

<script>
import BannerCom from './components/BannerCom.vue';
import HeaderComponent from './components/HeaderComponent.vue';

export default {
  components: { HeaderComponent, BannerCom }
}
</script>

<style lang="scss" scoped>

</style>