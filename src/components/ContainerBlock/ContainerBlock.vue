<template>
  <div class="container">
    <slot></slot>
  </div>
</template>

<script>
export default {
  name: "ContainerBlock",
};
</script>

<style scoped>
.container {
  background: rgba(255, 255, 255, 0.9);
  backdrop-filter: blur(6px);
  padding: 2%;
  box-shadow: 0px 10px 15px -3px rgba(0, 0, 0, 0.1);
  border-radius: 20px;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}
</style>
