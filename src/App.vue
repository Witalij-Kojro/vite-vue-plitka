<script setup>
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <div style="position: relative">
<base-nav type="default" effect="dark" expand>
    <a class="navbar-brand" href="#">Default Color</a>

    <div class="row" slot="content-header" slot-scope="{closeMenu}">
        <div class="col-6 collapse-brand">
            <a href="https://demos.creative-tim.com/vue-argon-design-system/documentation/">
                <img src="https://demos.creative-tim.com/vue-argon-design-system/img/brand/blue.png">
            </a>
        </div>
        <div class="col-6 collapse-close">
            <close-button @click="closeMenu"></close-button>
        </div>
    </div>

    <ul class="navbar-nav ml-lg-auto">
        <li class="nav-item">
            <a class="nav-link nav-link-icon" href="#">
                Discover
            </a>
        </li>
        <li class="nav-item">
            <a class="nav-link nav-link-icon" href="#">
                Profile
            </a>
        </li>
        <base-dropdown tag="li" title="Settings">
          <a class="dropdown-item" href="#">Action</a>
          <a class="dropdown-item" href="#">Another action</a>
          <a class="dropdown-item" href="#">Something else here</a>
          <div class="dropdown-divider"></div>
          <a class="dropdown-item" href="#">Separated link</a>
        </base-dropdown>
    </ul>
 </base-nav>
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
