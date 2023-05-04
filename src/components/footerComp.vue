<script>
    export default{
        name: "footerComp",
    }
</script>

<template>
    <footer>
        <div class="box">
            <div>
                <span class="signUp">
                    sign-up now!
                </span>
            </div>
            <div class="icon-box">
                <a href="#" class="follow">
                    follow us
                </a>
                <a href="https://www.facebook.com/dc/?locale=it_IT" target="_blank">
                    <img src="images/footer-facebook.png" alt="">
                </a>
                <a href="https://twitter.com/DCComics" target="_blank">
                    <img src="images/footer-twitter.png" alt="">
                </a>
                <a href="https://www.youtube.com/@dcofficial" target="_blank">
                    <img src="images/footer-youtube.png" alt="">
                </a>
                <a href="https://www.pinterest.it/dccomics/" target="_blank">
                    <img src="images/footer-pinterest.png" alt="">
                </a>
                <a href="#">
                    <img src="images/footer-periscope.png" alt="">
                </a>
            </div>

        </div>
        
    </footer>
</template>

<style lang="scss" scooped>
    @import '../style/partials/variables';

    footer{
        background-color: $grey;
        height: 150px;
        width: 100%;
        display: flex;
        align-items: center;
        .box {
            width: 80%;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            .signUp {
                color: white;
                text-transform: uppercase;
                font-size: 1.2rem;
                padding: 12px;
                border: 3px solid $blue-dc;
                
            }
            .icon-box {
                display: flex;
                justify-content: space-between;
                align-items: center; 
                a {
                    margin-right: 20px;
                }          
            }
            .follow {
                font-size: 1.5rem;
                text-transform: uppercase;
                text-decoration: none;
                color: $blue-dc;                    
            }

        }
    }
</style>