<template>
  <div class="my-2">
    <section>
      <h1>{{ title }}</h1>
      <div class="main-cards">
        <div class="button-div shadow">
          <button @click="scrollLeft">
            <ion-icon name="arrow-back-outline"></ion-icon>
          </button>
        </div>
        <div class="cards">
          <CardBlock v-for="card in cards" :key="card" :card="card" />
        </div>
        <div class="button-div shadow">
          <button @click="scrollRight">
            <ion-icon name="arrow-forward-outline"></ion-icon>
          </button>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import CardBlock from "../CardBlock/CardBlock.vue";

export default {
  name: "CardsScroll",
  props: {
    title: {
      type: String,
      default: "Título",
    },
    cards: {
      type: Array,
      default: () => [],
    },
  },
  methods: {
    scrollLeft() {
      const cards = this.$el.querySelector(".cards");
      cards.scrollLeft -= 300;
    },
    scrollRight() {
      const cards = this.$el.querySelector(".cards");
      cards.scrollLeft += 300;
    },
  },
  components: { CardBlock },
};
</script>

<style scoped>
section {
  margin-bottom: 4%;
  width: 90%;
  margin: 0 auto;
}

.main-cards {
  display: grid;
  grid-template-columns: 5% 90% 5%;
}

.card {
  width: 300px;
  height: 200px;
  flex: 0 0 auto;
}

.card img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  border-radius: 5px;
}

.card img:hover {
  filter: brightness(1.5);
  cursor: pointer;
}

.cards {
  display: flex;
  flex-wrap: nowrap;
  overflow-x: auto;
  gap: 2%;
  width: auto;
  -webkit-overflow-scrolling: touch;
  scroll-behavior: smooth;
}

.cards::-webkit-scrollbar {
  display: none;
}

h1 {
  color: var--dark;
  font-size: 28pt;
  font-weight: 900;
  padding-bottom: 2%;
}

.button-div {
  display: flex;
  align-items: center;
  height: 100%;
  width: 100%;
  background-color: rgb(255, 255, 255);
  opacity: 0.6;
  color: white;
  font-size: 24pt;
  font-weight: 900;
  backdrop-filter: blur(5px);
}

.button-div button {
  height: 100%;
  width: 100%;
  background: none;
  border: none;
}

@media (max-width: 768px) {
  .button-div {
    display: none;
  }

  .main-cards {
    grid-template-columns: 100%;
  }

  .card {
    width: 150px;
    height: 200px;
  }

  h1 {
    font-size: 18pt;
  }
}
</style>
