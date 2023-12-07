<script>
// Header
import HeaderComponent from './components/header/HeaderComponent.vue';
// Footer
import FooterComponent from './components/footer/FooterComponent.vue';
// Main
import ParteAzzurra from './components/main/ParteAzzurra.vue';

export default{
  components : {
    HeaderComponent,
    FooterComponent,
    ParteAzzurra
  }
}
</script>

<template>
  <HeaderComponent />
  <div class="black"><h2>Content goes here</h2></div>
  <main>
    <ParteAzzurra />
  </main>
  <FooterComponent />
</template>

<style scoped lang="scss">
@use './style/style.scss' as *;
  main {
    background-color: #0282F9;
    padding: 50px 0;

    > div {
        width: 1280px;
        margin: auto;
    }
  }
  .black{
      background-color: #1C1C1C;
      color: white;
      padding: 55px;
  }
</style>
