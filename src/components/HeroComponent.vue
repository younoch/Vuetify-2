<template>
  <v-container class="pt-15">
    <v-row>
      <v-col lg="6">
        <h2 class="intro-text">Welcome to our Vuetify App</h2>
        <p class="description">
          Lorem ipsum dolor sit, amet consectetur adipisicing elit. Ipsum
          blanditiis quod ad porro quaerat omnis temporibus eos nobis. Non
          officia sunt quidem voluptate velit consequuntur eos omnis id corporis
          aut.
        </p>
        <v-btn color="success" class="white--text mr-10" rounded
          >Get Started</v-btn
        >
        <v-btn color="indigo" class="white--text" rounded>
          <v-icon>mdi-play-circle</v-icon> Watch Video
        </v-btn>
      </v-col>
      <v-col>
        <img width="100%" src="./../assets/hero-img.png" alt="" />
      </v-col>
    </v-row>
  </v-container>
</template>
<script>
export default {
  name: "HeroComponent",
};
</script>

<style scoped>
.intro-text {
  font-size: 60px;
  font-weight: bold;
  font-family: cursive;
  color: #444;
}
.description {
  font-size: 19px;

  font-family: cursive;
  margin: 32px 0px;
  color: #444444ba;
}
</style>