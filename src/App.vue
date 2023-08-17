<template>
  <v-app>
    <v-app-bar
      app
      color="white"
      dark
    >
      <div class="d-flex align-center">
        <v-img
          alt="Ruka Star"
          class="shrink mr-2"
          contain
          src="../src/assets/logostar.png"
          transition="scale-transition"
          width="60"
          height="60"
        />

        <div class="font-weight-medium" style="color:#004D40">Ruka Star Limited</div>
      </div>

      <v-spacer></v-spacer>

      <div class="align-content-start" >
      <router-link to="/" class="font-weight-medium text-decoration-none " style="color:#004D40">
          Home
      </router-link>
      <router-link to="/about" class="font-weight-medium text-decoration-none" style="color:#004D40">
            About
        </router-link>
        </div>
    </v-app-bar>

    <v-main>
      <router-view/>
    </v-main>
  </v-app>
</template>

<script>

export default {
  name: 'App',

  data: () => ({
    //
  }),
};
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Poppins&display=swap');
</style>
