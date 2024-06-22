<script setup>
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <MDBNavbar expand="lg" light bg="light" container>
    <MDBNavbarBrand href="#">Brand</MDBNavbarBrand>
    <MDBNavbarToggler
      @click="collapse1 = !collapse1"
      target="#navbarSupportedContent"
    ></MDBNavbarToggler>
    <MDBCollapse v-model="collapse1" id="navbarSupportedContent">
      <MDBNavbarNav class="mb-2 mb-lg-0">
        <MDBNavbarItem to="#" active>
          Home
        </MDBNavbarItem>
        <MDBNavbarItem href="#">
          Link
        </MDBNavbarItem>
        <MDBNavbarItem>
          <!-- Navbar dropdown -->
          <MDBDropdown class="nav-item" v-model="dropdown1">
            <MDBDropdownToggle
              tag="a"
              class="nav-link"
              @click="dropdown1 = !dropdown1"
              >Dropdown</MDBDropdownToggle
            >
            <MDBDropdownMenu aria-labelledby="dropdownMenuButton">
              <MDBDropdownItem href="#">Action</MDBDropdownItem>
              <MDBDropdownItem href="#">Another Action</MDBDropdownItem>
              <MDBDropdownItem href="#"
                >Something else here</MDBDropdownItem
              >
            </MDBDropdownMenu>
          </MDBDropdown>
        </MDBNavbarItem>
        <MDBNavbarItem to="#" disabled>
          Disabled
        </MDBNavbarItem>
      </MDBNavbarNav>
      <!-- Search form -->
      <form class="d-flex input-group w-auto">
        <input
          type="search"
          class="form-control"
          placeholder="Type query"
          aria-label="Search"
        />
        <MDBBtn outline="primary">
          Search
        </MDBBtn>
      </form>
    </MDBCollapse>
  </MDBNavbar>
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
