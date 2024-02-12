<template>
  <nav class="navbar navbar-expand-lg">
    <div class="container-fluid container">
      <!-- Navbar -->
      <div class="d-flex justify-content-between w-100">
        <a class="navbar-brand text-white fs-2" href="#">Hex-Bits</a>
        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarNavDropdown"
          aria-controls="navbarNavDropdown"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>
      </div>
      <div class="collapse navbar-collapse" id="navbarNavDropdown">
        <ul class="navbar-nav">
          <li class="nav-item" v-for="(item, key) in items" :key="key">
            <a class="nav-link" :class="key == 0 ? 'active' : ''" aria-current="page" href="#">{{ item.name }}</a>
          </li>
        </ul>
      </div>
      <!-- Navbar -->
    </div>
  </nav>
</template>

<script setup>
const items = [
    {name: 'Inicio'},
    {name: 'Conocenos'},
    {name: 'Precios'},
    {name: 'Contacto'},
];
</script>

<style scoped>
nav {
  width: 100%;
  position: fixed;
  z-index: 2;
  font-weight: 300;
  padding: 30px;
  flex-direction: column;
}
.nav-link {
  color: rgb(212, 212, 212);
}
.active,
.nav-link:hover {
  color: white !important;
}
</style>