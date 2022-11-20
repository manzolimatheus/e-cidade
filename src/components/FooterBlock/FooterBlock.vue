<template>
  <footer>
    <div class="logo">
      <img src="/img/Logo.png" alt="Logo" />
    </div>
    <div class="text">
      <p>Mogi Mirim - SP - 2022</p>
    </div>
  </footer>
</template>

<script>
export default {
  name: "FooterBlock",
};
</script>

<style scoped>
footer {
  width: 100%;
  text-align: center;
  margin-top: 4%;
}

.logo, .text {
  padding: 2%;
}

.logo {
  background: var(--success);
}

.text {
  background: var(--success-dark);
}
</style>
