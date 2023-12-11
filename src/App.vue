<script>
// Header
import HeaderComponent from './components/header/HeaderComponent.vue';
// Footer
import FooterComponent from './components/footer/FooterComponent.vue';
// Main
import MainComponent from './components/main/MainComponent.vue';

export default{
  components : {
    HeaderComponent,
    FooterComponent,
    MainComponent
  }
}
</script>

<template>
  <HeaderComponent />
  <MainComponent />
  <FooterComponent />
</template>

<style scoped lang="scss">
@use './style/style.scss' as *;
</style>
