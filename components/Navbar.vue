<template>
<div>
    <v-navigation-drawer
      temporary
      v-model="drawer"
      fixed
      left
      app
    >
    <div class="container has-text-centered">
        <img id="handsomeBoi" src="~/assets/magrossetete.jpg">
        <v-divider></v-divider>
        <h1 class="title">19 years old</h1>
          <h2 class="subtitle"><v-icon>location_on</v-icon>Nice, France</h2>
    </div>
    </v-navigation-drawer>

  <v-toolbar dense fixed app>
      <v-tooltip bottom>
        <v-toolbar-side-icon @click.stop="drawer = !drawer" slot="activator">
        </v-toolbar-side-icon>
        <span>About</span>
      </v-tooltip>
      <v-toolbar-title>Mickaelicoptere</v-toolbar-title>
        <v-spacer></v-spacer>
      <router-link class="link" to="/">
      <v-tooltip bottom>
      <v-btn slot="activator" icon>
        <v-icon>home</v-icon>
      </v-btn>
      <span>Home</span>
      </v-tooltip>
      </router-link>
      <nuxt-link class="link" to="/projects">
      <v-tooltip bottom>
      <v-btn slot="activator" icon>
        <v-icon>apps</v-icon>
      </v-btn>
      <span>Projects</span>
      </v-tooltip>
      </nuxt-link>
      <nuxt-link  class="link" to="/contact">
      <v-tooltip bottom>
      <v-btn slot="activator" icon>
        <v-icon>mail</v-icon>
      </v-btn>
      <span>contacts</span>
      </v-tooltip>
      </nuxt-link>
  </v-toolbar>
 </div>
</template>

<style scoped>
#brand {
  display: flex;
  text-align: left;
  padding-top: 1em;
}
.link {
  color: black;
  background-image: linear-gradient(black, grey);
  background-size: 0 5px, auto;
  background-repeat: no-repeat;
  background-position: center bottom;
  transition: all 0.2s ease-out;
}
.link:hover {
  background-size: 100% 5px, auto;
}

#handsomeBoi {
  margin-top: 3rem;
  display: flex;
  align-items: center;
}
</style>

<script>
export default {
  data() {
    return {
      drawer: null
    };
  }
};
</script>
