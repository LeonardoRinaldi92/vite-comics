<script>
    export default {
        name: "thumbComics",
        props: ['dettagliThumb']
    }
</script>

<template>
    <div class="card">
        <div class="thumb">
            <img :src="dettagliThumb.thumb" alt="Y">
            <div class="price">
                <span>{{ dettagliThumb.price }}</span>
            </div>
        </div>   
        <span class="title">
            {{ dettagliThumb.series }}
        </span>
    </div>
</template>

<style lang="scss" scooped>
    .card {
        flex-basis:calc(100% / 6 );
        padding: 20px;
        .thumb {
            width: 100%;
            aspect-ratio: 1;
            overflow: hidden;  
            margin-bottom: 10px;  
            position: relative;
            &:hover .price{
                display: block;
            }     
            img {
                width: 100%;
                cursor: pointer;
            }
            .price {
                position: absolute;
                bottom: 0;
                color: white;
                background-color: black;
                display: none;
            }
        }
        .title {
            text-transform: uppercase;
            color: white;
            font-size: 0.75rem;
            line-height: 0.2rem;
            cursor: default;
        }
    }
</style>