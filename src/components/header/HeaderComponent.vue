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