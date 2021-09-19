<template>
  <v-app>
    <Header />

    <v-main>
      <HeroComponent />
      <AboutUs />
      <Portfolio />
    </v-main>
  </v-app>
</template>

<script>
import Header from "./components/Header.vue";
import HeroComponent from "./components/HeroComponent.vue";
import AboutUs from "./components/AboutUs.vue";
import Portfolio from "./components/Portfolio.vue";
export default {
  name: "App",
  components: {
    Header,
    HeroComponent,
    AboutUs,
    Portfolio,
  },
};
</script>
