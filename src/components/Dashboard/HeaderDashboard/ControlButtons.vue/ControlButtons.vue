<template>
  <div class="buttons col-2 p-4">
    <!-- Botões para Chamados, Notícias, Lojas e Configurações -->
    <router-link to="/" class="button-warning">🚨 Chamados</router-link>
    <router-link to="/" class="button-safe">📰 Notícias</router-link>
    <router-link to="/" class="button-success">🛒 Promoções</router-link>
    <router-link to="/" class="button-safe-dark">⚙ Configurações</router-link>
  </div>
</template>

<script>
export default {
  name: "ControlButtons",
};
</script>

<style scoped>
a {
  border-radius: 20px;
  padding: 1.5%;
  font-size: 14pt;
}

a:hover {
  filter: brightness(0.8);
}
</style>
