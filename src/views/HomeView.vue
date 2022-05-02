<template>

  <div class="home">
    <div class="container">
      
      <div class="intro box">
        <h3>We at <span>OG Roast</span> specialize in <span>everything Coffee.</span> 
        We do in-house roasting, hold tasting-events, have a shop and in our Café we offer 
        a large variety of delicious homemade cakes and pastries, and of course; our Coffee. You should drop by!</h3>
        <h1>COFFEE</h1>
      </div>

      <div class="photo box">
        <img src="../assets/coffee.jpg" alt="">
      </div>
      
    </div>
  </div>

</template>

<style scoped>
  .home{
    height: 100vh;
    width: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .container{
    position: relative;
    width: 90%;
    height: 80%;
  }

  .box{
    position: absolute;
    top: 0;
    width: 50%;
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .intro{
    left: 0;
    padding: 0 0 0 5px;
  }

  .box h3{
    text-align: justify;
    font-weight: 500;
    margin-top: 4vh;
    line-height: 1.3;
  }

  .box h3 span:nth-child(1){
    font-weight: 700;
    color: var(--bg-col);
    background: var(--font-col);
    padding: 2px 7px
  }

   .box h3 span{
    font-weight: 700;
  }

  .box h1{
    position: absolute;
    bottom: -100px;
    font-size: 313px;
    font-family: Bebas Neue;
  }

  .photo{
    right: 0;
  }

  .photo img{
    height: 100%;
    width: 80%;
    object-fit: cover;
  }
</style>