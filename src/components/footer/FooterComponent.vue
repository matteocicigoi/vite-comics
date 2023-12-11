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
<style scoped lang="scss">
    footer {
        background-image: url('/public/img/footer-bg.jpg');
    }
</style>