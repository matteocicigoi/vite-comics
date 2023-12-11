<script>
import ListaComponent from './ListaComponent.Vue';
export default {
    components : {
        ListaComponent
    }
};
</script>

<template>
    <div class="menu-footer"><ListaComponent /></div>
</template>
<style lang="scss">
    .menu-footer{
        height: 370px;
        padding-top: 45px;
        max-width: 1280px;
        margin: 0 auto;
        background-image: url('/public/img/dc-logo-bg.png');
        background-repeat: no-repeat;
        background-position: calc(1280px - 570px) -90px;
    }
</style>