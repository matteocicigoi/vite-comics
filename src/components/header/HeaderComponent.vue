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

<style lang="scss">
    header {
        display: flex;
        justify-content: space-between;
        align-items: center;

        ul {
            display: flex;
            list-style-type: none;

            li{
                padding: 18px;
                text-transform: uppercase;

                &.selected{
                    a{
                        color: #0282F9;
                    }
                }

                a{
                    text-decoration: none;
                    color: black;
                }
            }
        }
    }
</style>