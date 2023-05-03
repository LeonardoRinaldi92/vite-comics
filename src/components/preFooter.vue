<script>
    import Lista1 from './lista1.vue';
import lista1 from './lista1.vue'

    export default {
    name: "preFooter",
    component: {
        lista1,
    },
    components: { Lista1 }
}
</script>
<template>
    <div class="prefooter">
        <img src="/images/dc-logo-bg.png" id="logoBig" alt="">
        <div class="list">
            <div>
               <Lista1/>
            </div>
            <div></div>
            <div></div>

        </div>  
    </div>
</template>

<style lang="scss" scooped>
    .prefooter{
        height: 400px;
        width: 100%;
        background-image: url(/images/footer-bg.jpg);
        background-repeat: no-repeat;
        background-size: cover;
        position: relative;
        overflow: hidden;
        display: flex;
        #logoBig{
            position: absolute;
            top: -90%;
            transform: translate(0,+50%);
            left: 60%;
            .list {
                display: flex;
                div{
                    flex-basis: calc(100% / 3);
                }
            }
        }
    }
</style>