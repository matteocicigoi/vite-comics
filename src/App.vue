<script>
// Header
import HeaderComponent from './components/header/HeaderComponent.vue';
// Footer
import FooterComponent from './components/footer/FooterComponent.vue';

export default{
  components : {
    HeaderComponent,
    FooterComponent
  }
}
</script>

<template>
  <HeaderComponent />
  <FooterComponent />
</template>

<style scoped lang="scss">
@use './style/style.scss' as *;
</style>
