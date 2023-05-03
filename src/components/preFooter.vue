<script>
    import lista1 from './lista1.vue';
    import lista2 from './lista2.vue';
    import lista3 from './lista3.vue';


    export default {
    name: "preFooter",
    components: {
        lista1,
        lista2,
        lista3,
    },

}
</script>
<template>
    <div class="prefooter">
        <img src="/images/dc-logo-bg.png" id="logoBig" alt="">
        <div class="list">
            <div>
                <lista1/>
            </div>
            <div>
                <lista2/>
            </div>
            <div>
                <lista3/>
            </div>

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
        }
        .list {
            display: flex;
            margin-left: 10%;
            div {
                margin-right: 20px;
            }
        }
    }
</style>