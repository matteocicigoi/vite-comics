<script>
import SerieComponent from './SerieComponent.vue';
import dcComics from '../../assets/dc-comics.json';
import LoadMore from './LoadMore.vue';
export default {
    data() {
        return{
            series : dcComics
        }
    },
    components : {
        SerieComponent,
        LoadMore
    }
}
</script>
<template>
    <div>
        <ul>
            <SerieComponent v-for="serie in series" :img="serie.thumb" :title="serie.series" />
        </ul>
        <LoadMore />
    </div>
</template>
<style scoped lang="scss">
@use '/src/style/partials/variables.scss' as *;
div{
    background-color: $bg-series;
    color: $text-tertiary;
    padding: 55px;
    padding-bottom: 20px;

    ul {
        width: 1280px;
        margin: 0 auto;
        display: flex;
        flex-wrap: wrap;
        list-style-type: none;

        :deep(li){
            width: calc(100% / 6);
        }
    }
}
</style>