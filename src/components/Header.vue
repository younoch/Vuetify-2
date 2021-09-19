<template>
  <v-app-bar
    style="padding: 0px 90px"
    app
    color="white"
    light
    elevation="6"
    elevate-on-scroll
  >
    <v-toolbar-title>Vuetify App</v-toolbar-title>
    <v-spacer />
    <v-list class="d-flex align-center">
      <v-list-item
        link
        v-for="(manu, index) in manus"
        :key="index"
        :to="manu.route"
      >
        <v-list-item-title>{{ manu.title }}</v-list-item-title>
      </v-list-item>
      <v-btn text>
        <v-icon>mdi-magnify</v-icon>
      </v-btn>
      <v-btn outlined color="success"> Get Started</v-btn>
    </v-list>
  </v-app-bar>
</template>
<script>
export default {
  name: "Header",
  data() {
    return {
      manus: [
        { title: "Home", route: "home" },
        { title: "About us", route: "about-us" },
        { title: "Portfolio", route: "portfolio" },
        { title: "Project", route: "project" },
        { title: "Gallery", route: "gallery" },
        { title: "Contact", route: "contact" },
      ],
    };
  },
};
</script>
<style scoped>
v-toolbar-title {
  font-size: 32px;
  color: #4caf50;
  font-weight: 700;
  font-family: cursive;
}
</style>