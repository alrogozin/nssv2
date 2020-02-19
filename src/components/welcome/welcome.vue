<template>
  <div id="welcome">
    <h1>Блок с общей информацией</h1>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Veritatis, maiores reiciendis temporibus maxime cum excepturi, cupiditate tenetur exercitationem hic consectetur aliquid alias odit velit sapiente libero porro iure voluptates error mollitia commodi dolorem soluta ipsam nesciunt perferendis! Autem provident harum dolorem, rem perspiciatis cupiditate perferendis quasi nulla nemo quidem possimus?</p>
    <div class="cta">
      <router-link to="/signup">Регистрация</router-link>
      <router-link to="/signin">Войти</router-link>
    </div>
  </div>
</template>

<style scoped>
  #welcome {
    width: 80%;
    margin: auto;
  }

  h1 {
    text-align: center;
  }

  p {
    text-align: center;
  }

  .cta {
    width: 500px;
    margin: auto;
    text-align: center;
  }

  .cta a {
    margin: 10px;
    text-decoration: none;
    display: inline-block;
    border: 1px solid #521751;
    border-radius: 3px;
    width: 200px;
    padding: 10px;
    box-sizing: border-box;
    color: #521751;
  }

  .cta a:hover,
  .cta a:active {
    background-color: #521751;
    color: white;
  }
</style>