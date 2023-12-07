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
<style lang="scss">
    .footer-bottom{
        background-color: #303030;

        > div {
            max-width: 1280px;
            margin: 0 auto;
            justify-content: space-between;
            align-items: center;
            display: flex;
            padding: 20px 0;
        }
    }
</style>