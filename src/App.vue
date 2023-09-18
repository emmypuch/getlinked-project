<script setup>
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <div>
    <header>
      <div class="header-overlay">
        <img src="@/assets/images/purple-lens-header.svg" alt="Purple Lens Logo" />
      </div>
      <div class="logo">
        <img
          alt="GetLinked Logo"
          class="logo"
          src="@/assets/images/getlinked-logo.svg"
          width="125"
          height="125"
        />
      </div>

      <div class="wrapper">
        <nav>
          <RouterLink to="/">Home</RouterLink>
          <RouterLink to="/about">About</RouterLink>
        </nav>
      </div>
    </header>

    <RouterView />
    <HelloWorld />
  </div>
</template>

<style scoped>
header {
  background-color: #150e28;
  position: relative;
}

.header-overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 125px;
  height: 125px;
}
</style>
