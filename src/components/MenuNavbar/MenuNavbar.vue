<template>
  <header class="shadow">
    <nav>
      <RouterLink v-for="item in items" :key="item.icon" :to="item.route">
        <ion-icon :name="item.icon" />
        <p>{{ item.label }}</p>
      </RouterLink>
    </nav>
  </header>
  <span></span>
</template>

<script>
export default {
  name: "MenuNavbar",
  data() {
    return {
      items: [
        {
          label: "Início",
          icon: "home-outline",
          route: "/",
        },
        {
          label: "Notícias",
          icon: "newspaper-outline",
          route: "/",
        },
        {
          label: "Loja",
          icon: "cart-outline",
          route: "/",
        },
        {
          label: "Mais",
          icon: "ellipsis-vertical-outline",
          route: "/",
        },
      ],
    };
  },
};
</script>

<style scoped>
header {
  height: 100vh;
  width: 100px;
  position: fixed;
  background: white;
  z-index: 9999;
}

nav {
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-items: center;
  height: 100%;
  gap: 8%;
  text-align: center;
}

nav a {
  color: var(--dark);
}

@media (max-width: 768px) {
  header::before {
    content: "";
    margin-top: 100px;
  }

  header {
    height: 10vh;
    width: 100%;
    position: fixed;
    bottom: 0;
  }

  nav {
    flex-direction: row;
  }
}
</style>
