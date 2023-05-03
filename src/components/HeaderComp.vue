<script>
    export default{
        name: "HeaderComp",
        data() {
            return {
                navbar: [
                    {
                        menuName: "characters",
                        url: "/characters"
                    },
                    {
                        menuName: "comics",
                        url: "/comics"
                    },
                    {
                        menuName: "movies",
                        url: "/movies"
                    },
                    {
                        menuName: "tv",
                        url: "/tv"
                    },
                    {
                        menuName: "games",
                        url: "/games"
                    },
                    {
                        menuName: "collectibles",
                        url: "/collectibles"
                    },
                    {
                        menuName: "videos",
                        url: "/videos"
                    },
                    {
                        menuName: "fans",
                        url: "/fans"
                    },
                    {
                        menuName: "news",
                        url: "/news"
                    },
                    {
                        menuName: "shop",
                        url: "/characters"
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
                    <li v-for="(element,index) in navbar">
                        <a :href="element.url">
                            {{ element.menuName }}
                        </a>
                    </li>
                </ul>
            </nav>
        </header>
    </template>

    <style>
    </style>