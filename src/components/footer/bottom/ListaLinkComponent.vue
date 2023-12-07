<script>
export default {
    data(){
        return {
            name : 'follow us',
            link : [
                {
                    img : 'footer-facebook.png',
                    link : '#'
                },
                {
                    img : 'footer-twitter.png',
                    link : '#'
                },
                {
                    img : 'footer-youtube.png',
                    link : '#'
                },
                {
                    img : 'footer-pinterest.png',
                    link : '#'
                },
                {
                    img : 'footer-periscope.png',
                    link : '#'
                }
            ]
        }
    }
};
</script>

<template>
    <div class="links">
        <h2>{{ name }}</h2>
            <ul>
                <li v-for="element in link"><a :href="element.link"></a><img :src="`../../public/img/${element.img}`" alt="Link"></li>
            </ul>
    </div>
</template>