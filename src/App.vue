<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <header>
    <div class="wrapper">
      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </div>
  </header>
  <main>
    <RouterView />
  </main>
</template>

<style scoped>
header {
  height: 70px;
  background-color: aqua;
  display: flex;
  align-items: center;
  justify-content: center;
}

nav {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 16px;
  width: 100%;
  font-size: 16px;
}

main {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  width: 100%;
  height: 100%;
  background-color: #000;
  color: #fff;
}
</style>
