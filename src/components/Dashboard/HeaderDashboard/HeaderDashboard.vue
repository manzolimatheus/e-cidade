<template>
  <div class="text-center">
    <WeatherView />
    <h1>☔ Boa noite, Matheus</h1>
    <ControlButtons />
  </div>
</template>

<script>
import ControlButtons from "./ControlButtons.vue/ControlButtons.vue";
import WeatherView from "./WeatherView/WeatherView.vue";

export default {
  name: "HeaderDashboard",
  components: { WeatherView, ControlButtons },
};
</script>

<style></style>
