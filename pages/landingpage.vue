<template>
    <div>
        <v-container fluid full-height>
            <v-parallax :src="require('@/assets/hang5.png')" height="800">
            <v-layout
            column
            align-center
            justify-center>
            <!-- <p>button</p> -->
             <v-btn
              class="grey"
              dark
              large
              icon
              rounded>
              <v-icon>code</v-icon>
             </v-btn>
            </v-layout>
            </v-parallax>
            <landing-page-projects/>
            </v-container>
    </div>
</template>

<script>
import LandingPageProjects from '../components/LandingPageProjects'
export default {
    components: {
        LandingPageProjects
    }
    
}
</script>

<style>

</style>

