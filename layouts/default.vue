<template>
   <v-app>
     <!-- <v-toolbar dense fixed app>
      <v-toolbar-side-icon @click.stop="drawer = !drawer">
      </v-toolbar-side-icon>
      <v-toolbar-title>Mickaelicoptere</v-toolbar-title>
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
      </v-toolbar> -->
     <navbar/>
    <v-content>
        <nuxt/>
      <!-- <v-navigation-drawer
      temporary
      v-model="drawer"
      :clipped="clipped"
      fixed
      fluid
      app
    >
        <img src="~/assets/magrossetete.jpg">
        <v-divider></v-divider>
        <h1 class="title">19 years old</h1>
          <h2 class="subtitle"><v-icon>location_on</v-icon>Nice, France</h2>
    </v-navigation-drawer> -->
    </v-content>
    <issafooter/>
  </v-app>
</template> 

<script>
  import Navbar from '../components/Navbar'
  import issafooter from '../components/issaFooter'

  export default {
    data() {
    return {
      drawer: null,
      clipped: false
    };
  },  
    components: {
      Navbar,
      issafooter
    }
  }
</script>

<style>
html {
  font-family: "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*, *:before, *:after {
  box-sizing: border-box;
  margin: 0;
}

.button--green {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #3b8070;
  color: #3b8070;
  text-decoration: none;
  padding: 10px 30px;
}

.button--green:hover {
  color: #fff;
  background-color: #3b8070;
}

.button--grey {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #35495e;
  color: #35495e;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 15px;
}

.button--grey:hover {
  color: #fff;
  background-color: #35495e;
}
</style>
