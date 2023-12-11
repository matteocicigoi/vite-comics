<script>
export default {
    data() {
        return {
            lista : [
                {
                    title: 'dc comics',
                    element: [
                        {
                            name : 'Characters',
                            link : '#'
                        },
                        {
                            name : 'Comics',
                            link : '#'
                        },
                        {
                            name : 'Movies',
                            link : '#'
                        },
                        {
                            name : 'Tv',
                            link : '#'
                        },
                        {
                            name : 'Games',
                            link : '#'
                        },
                        {
                            name : 'Videos',
                            link : '#'
                        },
                        {
                            name : 'News',
                            link : '#'
                        }
                    ]

                },
                {
                    title: 'shop',
                    element: [
                        {
                            name : 'Shop Dc',
                            link : '#'
                        },
                        {
                            name : 'Shop Dc Collectibles',
                            link : '#'
                        }
                    ]

                },
                {
                    title: 'dc',
                    element: [
                        {
                            name : 'Therms Of Use',
                            link : '#'
                        },
                        {
                            name : 'Privacy policy (New)',
                            link : '#'
                        },
                        {
                            name : 'Ad Choices',
                            link : '#'
                        },
                        {
                            name : 'Advertsing',
                            link : '#'
                        },
                        {
                            name : 'Jobs',
                            link : '#'
                        },
                        {
                            name : 'Subscriptions',
                            link : '#'
                        },
                        {
                            name : 'Talent Workshops',
                            link : '#'
                        },
                        {
                            name : 'CPSC Certificates',
                            link : '#'
                        },
                        {
                            name : 'Ratings',
                            link : '#'
                        },
                        {
                            name : 'Shop Help',
                            link : '#'
                        },
                        {
                            name : 'Contact Us',
                            link : '#'
                        }
                    ]

                },
                {
                    title: 'sites',
                    element: [
                        {
                            name : 'DC',
                            link : '#'
                        },
                        {
                            name : 'MAD Magazine',
                            link : '#'
                        },
                        {
                            name : 'DC Kids',
                            link : '#'
                        },
                        {
                            name : 'DC Universe',
                            link : '#'
                        },
                        {
                            name : 'DC Power Visa',
                            link : '#'
                        }
                    ]

                }
            ]
        }
    }
};
</script>

<template>
    <ul class="list-footer">
        <li v-for="element in lista">
            <h2>{{ element.title }}</h2>
            <ul>
                <li v-for="page in element.element">
                    <a :href="page.link">{{ page.name }}</a>
                </li>
            </ul>
        </li>
    </ul>
</template>
<style lang="scss">
    .list-footer{
        display: flex;
        flex-direction: column;
        flex-wrap: wrap;
        justify-content: flex-start;
        width: max-content;
        height: 100%;
        list-style-type: none;
        gap: 30px;
        li {
            h2{
                color: white;
                text-transform: uppercase;
                margin-bottom: 10px;
            }
            ul {
                list-style-type: none;
                li{
                    padding: 2px;
                    a{
                        text-decoration: none;
                        color: #959595;
                        font-size: 14px;
                        &:hover{
                            color: #0282F9;
                        }
                    }
                }
            }
        }
    }
</style>