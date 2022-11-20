<template>
  <div>
    <div class="container-bg">
      <div class="temp">
        <h1>16º</h1>
        <p>Tempo Chuvoso</p>
        <p>Mogi Mirim</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "WeatherView",
};
</script>

<style scoped>
.container-bg {
  background: linear-gradient(to bottom, rgba(0, 0, 0, 0.4) 0%, var(--grey) 40%),
    url("https://media.tenor.com/f14xUacYc1oAAAAd/storm-world-meteorological-day.gif");
  background-attachment: fixed;
  background-repeat: no-repeat;
  background-size: cover;
  display: flex;
  justify-content: left;
  align-items: center;
  height: 40vh;
}

.temp {
  margin-left: 20%;
  color: white;
  font-size: 18pt;
}
</style>
