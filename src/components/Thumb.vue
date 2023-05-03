<script>
    export default{
        name: "Thumb",
    }
</script>
<template>
    <div class="Thumbbox">
        <div class="button">
            <span>
                load more
            </span>
        </div> 
    </div>
</template>

<style lang="scss" scoped>
    @import '../style/partials/variables';
    .Thumbbox{
        position: relative;
        .button {
            color: white;
            text-transform: uppercase;
            font-size: 1.2rem;
            background-color: $blue-dc;
            position: absolute;
            bottom: 0;
            padding: 10px 80px;
            bottom: 20px;
            left: 50%;
            transform: translate(-50% , 0);
            cursor: pointer;

        }
    }
</style>