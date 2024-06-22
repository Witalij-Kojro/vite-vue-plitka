<script setup>
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <div>
    <base-button type="primary" @click="modals.modal0 = true">
      Launch demo modal
    </base-button>
   <modal :show.sync="modals.modal0">
     <template slot="header">
        <h5 class="modal-title" id="exampleModalLabel">Modal title</h5>
     </template>
     <div>
      ...
     </div>
     <template slot="footer">
         <base-button type="secondary" @click="modals.modal0 = false">Close</base-button>
         <base-button type="primary">Save changes</base-button>
     </template>
   </modal>

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
