<script>
    export default {
        name: "lista3",
        data(){
            return {
                lista1: [
                    {
                        nomeLista: "sites",
                        links : [
                            {
                                name: "DC",
                                url: "https://www.dc.com"
                            },
                            {
                                name: "MAD magazine",
                                url: "https://www.madmagazine.com/"
                            },
                            {
                                name: "DC kids",
                                url: "https://www.dckids.com/"
                            },
                            {
                                name: "DC universe",
                                url: "https://www.dcuniverseinfinite.com/coming-soon/"
                            },
                            {
                                name: "DC power visa",
                                url: "https://www.bestcards.com/credit-cards/dc-power-visa/#:~:text=The%20DC%20Power%20Visa%C2%AE,well%20as%20dining%20and%20gas."
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
