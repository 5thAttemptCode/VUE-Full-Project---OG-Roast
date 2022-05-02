<template>

  <div class="ratio">
    <div class="coffee-amount">
      <p class="enter">Enter the desired amount of coffee</p>
      <input type="number" v-model="input" min="1">
      <label for="input">gr Coffee</label>
    </div>
    <br>
    <div class="input">
      <h3>French Press <span>4 min brew time</span></h3>
      <p class="water"> {{ input *14 }} gr Water</p>
    </div>
    <br>
    <div class="input">
      <h3>Pour Over <span>3-4 min brew time</span></h3>
      <p class="water"> {{ input *15 }} gr Water</p>
    </div>
  </div>

</template>


<script>
export default({
  data() {
    return {
      input: ''
    }
  }
})
</script>

<style scoped>

  .ratio{
    gap: 1vw;
    display: flex;
    flex-direction: column;
  }

  .input{
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 2vw;
    font-size: 20px;
  }

  input{
    width: 100px;
    padding: 10px;
    outline: none;
    border: none;
    font-size: 20px;
    background: white;
  }

  .water{
    padding: 10px;
    font-weight: 700;
    background: #7f227f;
    color: white;
    font-weight: 500;
    letter-spacing: 1px;
  }

  span{
    font-size: 16px;
    font-weight: 200;
    font-style: italic;
  }

  .enter{
    margin-bottom: 1vw;
  }

  label{
    margin-left: 1vw;
  }
</style>




