<script>
export default {
    data() {
        return {
            list: [
                {
                    name : 'digital comics',
                    link : '#',
                    img: 'buy-comics-digital-comics.png'

                },
                {
                    name : 'dc merchandise',
                    link : '#',
                    img: 'buy-comics-merchandise.png'

                },
                {
                    name : 'subscription',
                    link : '#',
                    img: 'buy-comics-subscriptions.png'

                },
                {
                    name : 'comic shop locator',
                    link : '#',
                    img: 'buy-comics-shop-locator.png'

                },
                {
                    name : 'dc power visa',
                    link : '#',
                    img: 'buy-dc-power-visa.svg'

                }
            ]
        }
    }
}
</script>

<template>
    <div>
        <ul class="list-element">
        <li v-for="element in list">
            <a :href="element.link">
                <div class="img">
                    <img :src="`/public/img/${element.img}`" :alt="element.name">
                </div>
                <span>{{ element.name }}</span>
            </a>
        </li>
    </ul>
    </div>
</template>
<style lang="scss">
    .list-element{
        list-style-type: none;
        display: flex;
        justify-content: space-around;
        width: 1280px;
        margin: auto;
        
        li {
            a {
                display: flex;
                align-items: center;
                text-decoration: none;
                
                .img {
                    height: 55px;
                    width: 55px;
                    display: block;
                    margin-right: 15px;

                    img {
                        object-fit: contain;
                        width: 100%;
                        height: 100%;
                    }
                }
                span {
                    text-transform: uppercase;
                    color: white;
                }
            }
        }
    }
</style>