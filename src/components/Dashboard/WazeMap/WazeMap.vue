<template>
  <div class="iframe-container">
    <iframe
      src="https://embed.waze.com/iframe?zoom=14&lat=-22.367939&lon=-46.943245&ct=livemap"
      height="450"
      frameborder="0"
      allowfullscreen
    ></iframe>
  </div>
</template>

<script>
export default {
  name: "WazeMap",
};
</script>

<style scoped>

.iframe-container {
    width: 90%;
    margin: 0 auto;
}

iframe {
    border-radius: 20px;
    width: 100%;
}

</style>
