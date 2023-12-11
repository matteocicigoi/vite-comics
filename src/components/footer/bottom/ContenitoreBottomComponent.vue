<script>
import SignUpComponent from './SignUpComponent.vue';
import ListaLinkComponent from './ListaLinkComponent.vue';
export default {
    components : {
        SignUpComponent,
        ListaLinkComponent
    }
};
</script>

<template>
    <div class="footer-bottom">
        <div>
            <SignUpComponent />
            <ListaLinkComponent />
        </div>
    </div>
</template>
<style scoped lang="scss">
@use '/src/style/partials/variables.scss' as *;
    .footer-bottom{
        background-color: $bg-footer;

        > div {
            max-width: $size;
            margin: 0 auto;
            justify-content: space-between;
            align-items: center;
            display: flex;
            padding: 20px 0;
        }
    }
</style>