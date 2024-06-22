<script setup>
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
<div class="bg-light text-center border-radius-lg py-4 mb-4">
  <h1 class="fw-bold">My First Bootstrap Page</h1>
  <p class="text-center">Resize this responsive page to see the effect!</p>
</div>

<div class="container">
  <div class="row">
    <div class="col-sm-4">
      <h3 class="fw-bold">Column 1</h3>
      <p>Lorem ipsum dolor..</p>
    </div>
    <div class="col-sm-4">
      <h3 class="fw-bold">Column 2</h3>
      <p>Lorem ipsum dolor..</p>
    </div>
    <div class="col-sm-4">
      <h3 class="fw-bold">Column 3</h3>
      <p>Lorem ipsum dolor..</p>
    </div>
  </div>
</div>

  <div>
    <a href="https://vitejs.dev" target="_blank">
      <img src="/vite.svg" class="logo" alt="Vite logo" />
    </a>
    <a href="https://vuejs.org/" target="_blank">
      <img src="./assets/vue.svg" class="logo vue" alt="Vue logo" />
    </a>
  </div>
  <HelloWorld msg="Укладка керамогранита в СПб." />
  Укладка широкоформаного керамогранита в Санкт-Петербурге.
  Укладка широкоформатного керамогранита 1200х600 в Санкт-Петербурге. Цена укладки широкоформатного кеерамогранита от 2800п за 1 м2.
  Механическая резка с водой, запилы под 45 градусов. Снятие кромки.
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
