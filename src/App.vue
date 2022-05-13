<template>
  <MainNavigation />
  <SubNavigation />
  <Carousel />
  <PlayerRadarChart />
  <PlayerDonutChart />
  <Partners />
  <Footer />
</template>

<script>
import MainNavigation from "./components/MainNavigation.vue";
import SubNavigation from "./components/SubNavigation.vue";
import Carousel from "./components/Carousel.vue";
import PlayerDonutChart from "./components/PlayerDonutChart.vue";
import PlayerRadarChart from "./components/PlayerRadarChart.vue";
import Partners from "./components/Partners.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    MainNavigation,
    SubNavigation,
    Carousel,
    PlayerDonutChart,
    PlayerRadarChart,
    Partners,
    Footer,
  },
};
</script>

<style>
</style>
