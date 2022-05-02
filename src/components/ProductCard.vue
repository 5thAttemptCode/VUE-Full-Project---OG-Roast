<template>
    <div class="coffe">
        <div class="photo">
            <img :src="kaffe.src" class="image" alt="">
        </div>
        <div class="heading">
            <h3 class="title">{{ kaffe.coffee }}</h3>
            <h3 class="origin">{{ kaffe.origin }}</h3>
            <p>{{ kaffe.description }}</p>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'ProductCard',
        props: ['kaffe']
    }
</script>

<style scoped>
    .coffe{
        position: relative;
        width: 33.33%;
        height: 100%;
        background: var(--pc-col);
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        transition: all 0.6s;
    }

    .coffe:hover{
        box-shadow: 5px 5px 15px 5px #000000;
        transform: translateY(-3px) scale(1.01);
    }

    .coffe:nth-child(1):hover{
        background: #141414;
        color: rgb(227, 151, 11);
    }

    .coffe:nth-child(2):hover{
        background: #742b74;
        color: rgb(95, 171, 241);
    }

    .coffe:nth-child(3):hover{
        background: #294e50;
        color: rgb(230, 110, 128);
    }

    .photo{
        width: 100%;
        height: 50%;
    }

    .photo img{
        height: 100%;
        width: 100%;
        object-fit: contain;
    }

    .heading{
        width: 100%;
        height: 50%;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
        gap: 2vh;
    }

    .title{
        letter-spacing: 1px;
    }

    .origin{
        font-style: italic;
        font-weight: 400;
    }

    h3{
        font-family: Bebas Neue;
        font-size: 25px;
    }

    p{
        text-align: justify;
        padding: 0 2vw;
    }
</style>