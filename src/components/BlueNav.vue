<script>
    export default {
        name: "BlueNav",
        data() {
            return {
                path: "/images/",
                icons:[
                    {
                        name: "digital comics",
                        url:"buy-comics-digital-comics.png",
                    },
                    {
                        name: "dc merchandise",
                        url:"buy-comics-merchandise.png",
                    },
                    {
                        name: "subscription",
                        url:"buy-comics-subscriptions.png",
                    },
                    {
                        name: "comic shop locator",
                        url:"buy-comics-shop-locator.png",
                    },
                    {
                        name: "dc power visa",
                        url:"buy-dc-power-visa.svg",
                    },   
                ]
            }
        },
    }
</script>

<template>
    <div class="bluenav">
        <div class="box-size">
            <div v-for="(element,index) in icons" class="icon">
                <img :src="path+element.url" alt="" :id="(element.url.includes('svg')? 'icon-img':'' )">
                <span>
                    {{ element.name }}
                </span>
            </div>
        </div>      
    </div>
</template>

<style>
</style>