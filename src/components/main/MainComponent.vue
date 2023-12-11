<script>
import JumboComponent from './JumboComponent.vue';
import CurrentSeriesComponent from './CurrentSeriesComponent.vue';
import ShopComponent from './ShopComponent.vue';
import SeriesComponent from './SeriesComponent.vue';
export default {
    components : {
        ShopComponent,
        JumboComponent,
        CurrentSeriesComponent,
        SeriesComponent
    }
}
</script>
<template>
    <main>
        <JumboComponent />
        <CurrentSeriesComponent />
        <SeriesComponent />
        <ShopComponent />
        
    </main>
</template>
<style scoped lang="scss">
main {
    position: relative;
}
</style>
