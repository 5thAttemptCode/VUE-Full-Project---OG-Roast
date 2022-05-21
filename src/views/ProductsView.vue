<template>

    <div class="products">
        <h3>All our Coffee Beans are available in our Café, just ask our staff. <br> Check out our <a href="./about">Coffee Calculator</a> for the perfect coffee experience at home!</h3>
        <div class="products-inner">
            <ProductCard v-for="kaffe in cafe" :key="kaffe.coffee" :kaffe="kaffe"></ProductCard> 
        </div>
    </div>
    
</template>

<script>
import ProductCard from '@/components/ProductCard.vue'

export default {
  name: 'ProductsView',
  components: {
    ProductCard: ProductCard
  },
  data: () => {
            return {
             cafe: 
                [
                    {coffee: 'Dark C4 Xpresso', origin: 'from Ethiopia', description: 'Dark, bold, explosive; our C4 espresso coffee beans are not for the weak hearted. Dark chocolate notes, tobaco aroma and a hint of citrus.', src: require('../assets/1.png')},
                    {coffee: 'Beach Blend Light Roast', origin: 'from Costa Rica', description: 'Beach Blend is the perfect allrounder coffee bean. Relaxed morning, chilled afternoon or just to keep you up for that over time.', src: require('../assets/2.png')},
                    {coffee: 'Cubano Coffee Medium', origin: 'from Cuba', description: 'High acidity and slightly sweet. The Cubano Coffee is for those who enjoy that extra little something in their daily coffee.', src: require('../assets/3.png')}
                ]
            }
        }

}
</script>

<style scoped>
    .products{
        height: 100vh;
        width: 100%;
        display: flex;
        flex-direction: column;
        gap: 5vh;
        justify-content: center;
        align-items: center;
    }

    .products-inner{
        position: relative;
        width: 90%;
        height: 65%;
        padding: 0 7.5vw;
        display: flex;
        gap: 5%;
        justify-content: center;
        align-items: center;
    }

    h3{
        margin-left: 34vw;
        font-weight: 500;
        line-height: 1.5;
        text-align: right;
    }

    h3 a{
        font-weight: 600;
        background: var(--con-col);
        color: var(--hov-col);
        padding: 1px 5px;
        text-transform: uppercase;
        transition: all 0.4s;
    }

    h3 a:hover{
        color: var(--con-col);
        background: var(--hov-col);
    }

</style>