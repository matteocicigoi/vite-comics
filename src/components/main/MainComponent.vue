<script>
import JumboComponent from './JumboComponent.vue';
import CurrentSeriesComponent from './CurrentSeriesComponent.vue';
import ShopComponent from './ShopComponent.vue';
export default {
    components : {
        ShopComponent,
        JumboComponent,
        CurrentSeriesComponent
    }
}
</script>
<template>
    <main>
        <JumboComponent />
        <CurrentSeriesComponent />
        <div class="black"><h2>Content goes here</h2></div>
        <ShopComponent class="shop"/>
    </main>
</template>
<style lang="scss">
main {
    position: relative;
}
.shop {
    background-color: #0282F9;
    padding: 50px 0;
}
.black{
    background-color: #1C1C1C;
    color: white;
    padding: 55px;
}
</style>
