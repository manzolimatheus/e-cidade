<template>
  <div class="col">
    <MenuNavbarVue />
    <RouterView />
  </div>
  <FooterBlock />
</template>

<script setup>
import { RouterLink, RouterView } from "vue-router";
import MenuNavbarVue from "./components/MenuNavbar/MenuNavbar.vue";
import FooterBlock from "./components/FooterBlock/FooterBlock.vue";
</script>

<style scoped>
.col {
  display: grid;
  grid-template-columns: 6% 94%;
}

@media (max-width: 768px) {
  .col {
    grid-template-columns: 100%;
  }
}
</style>
