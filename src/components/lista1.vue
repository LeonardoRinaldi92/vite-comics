<script>
    export default {
        name: "lista1",
        data(){
            return {
                lista1: [
                    {
                        nomeLista: "dc comics",
                        links : [
                            {
                                name: "characters",
                                url: "/characters"
                            },
                            {
                                name: "comics",
                                url: "/comics"
                            },
                            {
                                name: "movies",
                                url: "/movies"
                            },
                            {
                                name: "tv",
                                url: "/tv"
                            },
                            {
                                name: "games",
                                url: "/games"
                            },
                            {
                                name: "videos",
                                url: "/videos"
                            },
                            {
                                name: "news",
                                url: "/news"
                            }
                        ],
                    }
                ],
                lista2 : [
                    {
                        nomeLista: "shop",
                        links: [
                            {
                                name: "shop DC",
                                url: "/shop_dc" 
                            },
                            {
                                name:"shop DC Collectibles",
                                url:"/shop_dc_collectibles"
                            }
                        ]

                    }
                ]
            }
        }
    }
</script>
<template>
    <div>
        <span class="list-title">
            {{lista1[0].nomeLista}}
        </span>
        <ul class="lista-bottom"> 
            <li v-for="(element,index) in lista1[0].links">
                <a :href="element.url">
                {{ element.name }}
                </a>
            </li>
        </ul>       
    </div>
    <div>
        <span class="list-title">
            {{lista2[0].nomeLista}}
        </span>
        <ul class="lista-bottom"> 
            <li v-for="(element,index) in lista2[0].links">
                <a :href="element.url">
                {{ element.name }}
                </a>
            </li>
        </ul>       
    </div>
</template>
<style>
</style>