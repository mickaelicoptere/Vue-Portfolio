<template>
    <div>
        <v-content fluid fill-height>
            <v-parallax src="/images/hang5.png" height="900">
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
            </v-content>
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

