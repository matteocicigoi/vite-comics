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
    }
</style>