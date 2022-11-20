<template>
  <div class="card" :style="cardStyle">
    <p>{{ card.description }}</p>
  </div>
</template>

<script>
export default {
  name: "CardBlock",
  props: {
    card: {
      type: Object,
      default: () => {},
    },
  },
  computed: {
    cardStyle() {
      //   Background = card.image, Dark Gradient = rgba(0, 0, 0, 0.5), no-repeat, cover
      return `background: url(${this.card.image}) rgba(0, 0, 0, 0.5) no-repeat center center / cover`;
    },
  },
};
</script>

<style scoped>
.card {
  display: flex;
  justify-content: center;
  align-items: center;
  color: white;
  border-radius: 20px;
  margin-left: 2%;
}

.card hover {
  cursor: pointer;
  filter: brightness(0.8);
}
</style>
