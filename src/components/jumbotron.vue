<script>
    export default{
        name: "jumbotron",
    }
</script>
<template>
    <div id="jumbo">
        <div class="current">
            current series
        </div>
        
    </div>
</template>

<style lang="scss" scoped>
    @import '../style/partials/variables';
    #jumbo {
        height: 400px;
        width: 100%;
        background-image: url(../../public/images/jumbotron.jpg);
        background-repeat: no-repeat;
        position: relative;
        .current {
            position: absolute;
            padding: 15px 30px;
            bottom: -30px;
            left: 15%;
            color: white;
            text-transform: uppercase;
            font-size: 1.5rem;
            background-color: $blue-dc;
            cursor: pointer;

        }
    }
</style>