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