<script>
import LogoComponent from './LogoComponent.vue';
import MenuComponent from './MenuComponent.vue';

export default {
    components : {
        LogoComponent,
        MenuComponent
    }
};
</script>

<template>
    <header>
        <LogoComponent />
        <MenuComponent />
    </header>
</template>

<style scoped lang="scss">
@use '/src/style/partials/variables.scss' as *;
    header {
        display: flex;
        justify-content: space-between;
        align-items: center;
        max-width: $size;
        margin: 0 auto;
        padding: 20px 0;
    }
</style>