<template>
  <nav>
    <ul>
      <router-link to="/">OG Roast</router-link> |
      <router-link to="/product">Products</router-link> |
      <router-link to="/about">Calculator</router-link>
    </ul>
  </nav>
  <router-view/>
</template>

<style>
@import url("https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Roboto:wght@300;400;500&display=swap");

*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  text-decoration: none;
  font-family: Roboto;
}

:root{
  --bg-col: rgb(202, 145, 84);
  --pc-col: rgb(173, 119, 61);
  --font-col: #141414;
  --hov-col: beige;
}

body{
  background: var(--bg-col);
  overflow-y: hidden;
}

#app {
  height: 100vh;
  width: 100%;
}

nav {
  position: fixed;
  width: 100%;
  height: 10vh;
  z-index: 100;
  display: flex;
  justify-content: left;
  align-items: center;
  padding-left: 5vw;
}

nav ul{
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  width: 30vw;
}

nav a{
  font-weight: bold;
  color: var(--font-col);
  transition: all 0.4s;
}

nav a:hover{
  color: var(--hov-col);
}

nav a:nth-of-type(1){
  border: 2px solid var(--font-col);
  padding: 5px 10px;
}

nav a:nth-of-type(1):hover{
  border: 2px solid white;
  padding: 5px 10px;
}

</style>
