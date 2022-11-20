<template>
  <div>
    <CardsScroll :title="title" :cards="cards" />
  </div>
</template>

<script>
import CardsScroll from "../../CardsScroll/CardsScroll.vue";

export default {
  name: "RecentNews",
  data() {
    return {
      cards: [
        {
          image:
            "https://www.teclasap.com.br/wp-content/uploads/2014/09/fish.jpg",
          description: "Hello World",
        },
        {
          image:
            "https://www.teclasap.com.br/wp-content/uploads/2014/09/fish.jpg",
          description: "Hello World",
        },
        {
          image:
            "https://www.teclasap.com.br/wp-content/uploads/2014/09/fish.jpg",
          description: "Hello World",
        },
        {
          image:
            "https://www.teclasap.com.br/wp-content/uploads/2014/09/fish.jpg",
          description: "Hello World",
        },
        {
          image:
            "https://www.teclasap.com.br/wp-content/uploads/2014/09/fish.jpg",
          description: "Hello World",
        },
        {
          image:
            "https://www.teclasap.com.br/wp-content/uploads/2014/09/fish.jpg",
          description: "Hello World",
        },
        {
          image:
            "https://www.teclasap.com.br/wp-content/uploads/2014/09/fish.jpg",
          description: "Hello World",
        },
        {
          image:
            "https://www.teclasap.com.br/wp-content/uploads/2014/09/fish.jpg",
          description: "Hello World",
        },
      ],
      title: "Notícias Recentes",
    };
  },
  components: { CardsScroll },
};
</script>

<style scoped></style>
