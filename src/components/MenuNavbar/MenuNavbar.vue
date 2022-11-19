<template>
  <header>
    <nav>
      <RouterLink v-for="item in items" :key="item.icon" :to="item.route">
        <ion-icon :name="item.icon"/>
        <p>{{item.label}}</p>
      </RouterLink>
    </nav>
  </header>
</template>

<script>
export default {
  name: "MenuNavbar",
  data() {
    return {
      items: [
        {
          label: 'Início',
          icon: 'home-outline',
          route: '/'
        },
        {
          label: 'Notícias',
          icon: 'newspaper-outline',
          route: '/'
        },
        {
          label: 'Loja',
          icon: 'cart-outline',
          route: '/'
        },
        {
          label: 'Mais',
          icon: 'ellipsis-vertical-outline',
          route: '/'
        },
      ]
    }
  },
};
</script>

<style scoped>

header {
  border: 2px solid grey;
  height: 100vh;
  width: 4%;
}

nav {
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-items: center;
  height: 100%;
  gap: 10%;
  text-align: center;
}

</style>
