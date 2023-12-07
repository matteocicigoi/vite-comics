<script>
export default {
    data(){
        return {
            menu : [
                {
                    name : 'characters',
                    link : '#'
                },
                {
                    name : 'comics',
                    link : '#'
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
    }
};
</script>

<template>
<ul>
<li v-for="element in menu"><a :href="element.link">{{ element.name }}</a></li>
</ul>
</template>