<template>

  <div class="about">
    <div class="about-inner">
      <div class="text box">
        <h1>Why is Coffee Water ratio <br> so important?</h1>
        <p>A coffee’s flavor will vary depending on the technique used to make it. 
        Think of it as you would any other recipe; it is a delicate art, and each 
        ingredient you use matters. By increasing or decreasing the amount of water 
        or coffee beans you use, you can alter the taste and the viscosity of the 
        beverage. This is why baristas and coffee enthusiasts alike often use scales 
        and timers when brewing. <br> <br>
        Some baristas swear by recipes such as “60 grams of coffee per liter of water for so 
        many cups.” But others will instead focus on ratios. Understanding these ratios is simple. If 
        you have 1g of coffee and 1g of water, the ratio of coffee to water is 1:1. If you 
        have 1g of coffee and 15g of water, the ratio is 1:15. But nobody brews a 15g cup of coffee, 
        which is way too small for the much-needed caffeine hit. What is more common is a 
        350g cup of coffee. No matter the brew ratio, most baristas will aim to keep it 
        consistent. This is so that they can work effectively and efficiently and so that 
        if they like how coffee tastes, they can easily replicate it in the future.</p>
      </div>
      <div class="calculator box">
        <h1>Coffee Water Ratio Calculator</h1>
        <CoffeeTime></CoffeeTime>
      </div>
    </div>
  </div>
</template>

<script>
import CoffeeTime from '@/components/CoffeeTime.vue'


export default {
  name: 'AboutView',
  components: {
    CoffeeTime: CoffeeTime
  },
}
</script>

<style scoped>
  .about{
    height: 100vh;
    width: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .about-inner{
    position: relative;
    width: 85%;
    height: 80%;
    margin-top: 10vh;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .box{
    height: 100%;
    width: 50%;
    padding: 2vw 3vw;
  }

  .text{
    text-align: justify;
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
    align-items: left;
    line-height: 1.3;
  }

  h1{
    font-size: 40px;
    font-family: Bebas Neue;
  }

  p{
    font-size: 17px;
  }

  .calculator{
    padding: 3vw 3vw 3vw 7vw;
    display: flex;
    gap: 2vw;
    flex-direction: column;
    justify-content: top;
    align-items: left;
  }
</style>
