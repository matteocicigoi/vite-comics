<script>
import ContenitoreComponent from './menu/ContenitoreComponent.Vue';
import ContenitoreBottomComponent from './bottom/ContenitoreBottomComponent.vue';
export default {
    components : {
        ContenitoreComponent,
        ContenitoreBottomComponent
    }
};
</script>

<template>
    <footer>
        <ContenitoreComponent />
        <ContenitoreBottomComponent />
    </footer>
</template>
<style lang="scss">
    footer {
        background-image: url('/public/img/footer-bg.jpg');
        
        .menu-footer{
            max-width: 1280px;
            margin: 0 auto;
            background-image: url('/public/img/dc-logo-bg.png');
            background-repeat: no-repeat;
            background-position: calc(1280px - 570px) -90px;
        }
    }
</style>