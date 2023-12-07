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
                padding: 0 18px;
                text-transform: uppercase;

                &.selected{
                    a{
                        color: #0282F9;
                    }
                    a::after{
                        content: '';
                        display: block;
                        width: 100%;
                        height: 5px;
                        position: absolute;
                        top: 76px;
                        background-color: #0282F9;
                    }
                }

                a{
                    text-decoration: none;
                    color: black;
                    position: relative;
                    line-height: 103px;
                }
            }
        }
    }
</style>