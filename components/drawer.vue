<template>
<v-toolbar-side-icon @click.stop="drawer = !drawer">
            <v-navigation-drawer
                  temporary
                  v-model="drawer"
                  absolute
                >
                  <v-list class="pa-1">
                    <v-list-tile avatar>
                      <v-list-tile-avatar>
                        <img src="https://randomuser.me/api/portraits/men/85.jpg" >
                      </v-list-tile-avatar>
                      <v-list-tile-content>
                        <v-list-tile-title>John Leider</v-list-tile-title>
                      </v-list-tile-content>
                    </v-list-tile>
                  </v-list>
                </v-navigation-drawer>
      </v-toolbar-side-icon>
</template>

<script>
  export default {
    props:() => {
        drawer: null
    },
    data () {
      return {
        drawer: null,
      }
    }
  }
</script>