<script>
import LogoComponent from './LogoComponent.vue';
import ContenitoreComponent from './menu/ContenitoreComponent.Vue';
import ContenitoreBottomComponent from './bottom/ContenitoreBottomComponent.vue';
export default {
    components : {
        LogoComponent,
        ContenitoreComponent,
        ContenitoreBottomComponent
    }
};
</script>

<template>
    <ContenitoreComponent />
    <LogoComponent />
    <ContenitoreBottomComponent />
</template>