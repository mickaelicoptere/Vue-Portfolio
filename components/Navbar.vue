<template>
  <!-- <div class="container">
    <nav class="navbar" role="navigation" aria-label="main navigation">
      <div class="navbar-brand">
        <p id='brand'>Mickaelicoptere</p>
        <button class="button navbar-burger">
        </button>
      </div>
      <div class="navbar-menu">
        <div class="navbar-end">
          <nuxt-link class="navbar-item" to="/">Home</nuxt-link>
          <nuxt-link class="navbar-item" to="/about">About</nuxt-link>
          <nuxt-link class="navbar-item" to="/projects">Projects</nuxt-link>
          <nuxt-link class="navbar-item" to="/contact">Contact</nuxt-link>
        </div>
      </div>
    </nav>
  </div> -->
  <v-toolbar dense>
      <nuxt-link class="link" to="/about">
      <v-toolbar-side-icon>
      </v-toolbar-side-icon>
      </nuxt-link>
      <v-toolbar-title>Mickael Lanier's portfolio</v-toolbar-title>
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
</style>