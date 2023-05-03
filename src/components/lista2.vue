<script>
    export default {
        name: "lista2",
        data(){
            return {
                lista1: [
                    {
                        nomeLista: "dc",
                        links : [
                            {
                                name: "term of use",
                                url: "/term_of_use"
                            },
                            {
                                name: "privacy policy(new)",
                                url: "/privacy_policy"
                            },
                            {
                                name: "ad choices",
                                url: "/ad_choices"
                            },
                            {
                                name: "advertsing",
                                url: "/advertsing"
                            },
                            {
                                name: "jobs",
                                url: "/jobs"
                            },
                            {
                                name: "subscriptions",
                                url: "/subscriptions"
                            },
                            {
                                name: "talent workshop",
                                url: "/talent_workshop"
                            },
                            {
                                name: "CPSCS certificate",
                                url: "/CPSCS_certificate"
                            },
                            {
                                name: "talent workshop",
                                url: "/talent_workshop"
                            },
                            {
                                name: "ratings",
                                url: "/ratings"
                            },
                            {
                                name: "shop help",
                                url: "/shop help"
                            },
                            {
                                name: "contact us",
                                url: "/contact us"
                            },
                        ],
                    }
                ],
                
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
</template>