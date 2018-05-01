<template>
<div>

  <v-toolbar dense>
      <!-- <nuxt-link class="link" to="/about"> -->
      <v-toolbar-side-icon @click.stop="drawer = !drawer">
        
      </v-toolbar-side-icon>
      <!-- </nuxt-link> -->
      <v-toolbar-title class=".display-3">Mickael Lanier's portfolio</v-toolbar-title>
      <v-spacer></v-spacer>
        
      <router-link class="link" to="/">
      <v-btn icon>
        <v-icon>home</v-icon>
      </v-btn>
      </router-link>


      <nuxt-link class="link" to="/projects">
      <v-btn icon>
        <v-icon>apps</v-icon>
      </v-btn>
      </nuxt-link>
      <nuxt-link  class="link" to="/contact">
      <v-btn icon>
        <v-icon>mail</v-icon>
      </v-btn>
      </nuxt-link>
    </v-toolbar>

 <v-layout wrap>
 <v-navigation-drawer
      temporary
      v-model="drawer"
      absolute
    >
    <div class="container has-text-centered">
        <img id="handsomeDude" src="~/assets/magrossetete.jpg">
        <v-divider></v-divider>
        <h1 class="title">19 years old</h1>
          <h2 class="subtitle"><v-icon>location_on</v-icon>Nice, France</h2>
    </div>
    </v-navigation-drawer>
 </v-layout>


</div>
</template>

<style>
#brand {
  display: flex;
  text-align: left;
  padding-top: 1em;
}
.link {
  color: black;
}
#handsomeDude {
  margin: 3em 3em 3em 3em;
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
