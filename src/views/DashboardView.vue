<template>
  <div>
    <HeaderDashboard />
    <WazeMap />
    <RecentNews />
  </div>
</template>

<script>
import HeaderDashboard from '../components/Dashboard/HeaderDashboard/HeaderDashboard.vue';
import WazeMap from '../components/Dashboard/WazeMap/WazeMap.vue';
import RecentNews from '../components/NewsCards/RecentNews/RecentNews.vue';

export default {
  name: "DashboardView",
  components: { HeaderDashboard, WazeMap, RecentNews },
};
</script>

<style></style>
