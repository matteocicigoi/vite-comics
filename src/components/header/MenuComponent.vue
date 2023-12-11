<script>
import { callWithAsyncErrorHandling } from 'vue';

export default {
    data(){
        return {
            selected : 1,
            menu : [
                {
                    name : 'characters',
                    link : '#',
                },
                {
                    name : 'comics',
                    link : '#',
                },
                {
                    name : 'movies',
                    link : '#'
                },
                {
                    name : 'tv',
                    link : '#'
                },
                {
                    name : 'games',
                    link : '#'
                },
                {
                    name : 'collectibles',
                    link : '#'
                },
                {
                    name : 'videos',
                    link : '#'
                },
                {
                    name : 'fans',
                    link : '#'
                },
                {
                    name : 'news',
                    link : '#'
                },
                {
                    name : 'shop',
                    link : '#'
                }
            ]
        }
    },
    methods : {
        select(index){
            this.selected = index;
        }
    }
};
</script>

<template>
<ul>
<li v-for="(element, index) in menu" :class="{selected : index === selected}" @click="select(index)"><a :href="element.link">{{ element.name }}</a></li>
</ul>
</template>
<style scoped lang="scss">
@use '/src/style/partials/variables.scss' as *;
ul {
    display: flex;
    list-style-type: none;

    li{
        padding: 0 18px;
        text-transform: uppercase;

        &.selected{
            a{
                color: $text-primary;
            }
            a::after{
                content: '';
                display: block;
                width: 100%;
                height: 5px;
                position: absolute;
                top: 76px;
                background-color: $br-primary;
            }
        }

        a{
            text-decoration: none;
            color: $text-secondary;
            position: relative;
            line-height: 103px;
            
            &:hover{
                color: $text-primary
            }
        }
    }
}
</style>