<script>
    export default{
        name: "HeaderComp",
        data() {
            return {
                navbar: [
                    {
                        menuName: "characters",
                        url: "/characters",
                        visible: false
                    },
                    {
                        menuName: "comics",
                        url: "/comics",
                        visible: true
                    },
                    {
                        menuName: "movies",
                        url: "/movies",
                        visible: false
                    },
                    {
                        menuName: "tv",
                        url: "/tv",
                        visible: false
                    },
                    {
                        menuName: "games",
                        url: "/games",
                        visible: false
                    },
                    {
                        menuName: "collectibles",
                        url: "/collectibles",
                        visible: false
                    },
                    {
                        menuName: "videos",
                        url: "/videos",
                        visible: false
                    },
                    {
                        menuName: "fans",
                        url: "/fans",
                        visible: false
                    },
                    {
                        menuName: "news",
                        url: "/news",
                        visible: false
                    },
                    {
                        menuName: "shop",
                        url: "/characters",
                        visible: false
                    },
                ]            
            }
        }
    }
</script>

<template>
    <header>
        <div id="logo">
            <img src="/images/dc-logo.png" alt="">
        </div>
        <nav>
            <ul>
                <li v-for="(element,index) in navbar" :class="element.visible ? 'active' : ''">
                    <a :href="element.url">
                        <b>
                            {{ element.menuName }}
                        </b>
                    </a>
                </li>
            </ul>
        </nav>
    </header>
</template>
<style>
</style>