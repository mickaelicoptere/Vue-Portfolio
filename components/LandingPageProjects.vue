<template>
            <v-layout column align-center justify-center>
            <h1 id="title">Landing Page !!</h1>
            <v-flex xs12>
                <v-container grid-list-xl>
                <v-layout row wrap align-center>
                    <v-flex xs12 md4 v-for="p in projects" :key="p">
                        <v-card class="elevation-0 transparent">
                            <v-card-text class="text-xs-center">
                                <v-icon x-large class="blue--text text--lighten-2">{{p.icon}}</v-icon>
                            </v-card-text>
                            <v-card-title primary-title class="layout justify-center">
                                <div class="headline text-xs-center">{{p.title}}</div>
                            </v-card-title>
                            <v-card-text>
                                {{p.text}}
                            </v-card-text>
                        </v-card>
                    </v-flex>
                </v-layout>
            </v-container>
         </v-flex>
    </v-layout>
</template>

<script>
export default {
    data: () => ({
        projects: [
            {
                icon: "color_lens",
                title: "Material Design Askip",
                text: "Cras facilisis mi vitae nunc lobortis pharetra. Nulla volutpat tincidunt ornare. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis Nullam in aliquet odio. Aliquam eu est vitae tellus bibendum tincidunt. Suspendisse potenti."
            },
            {
                icon: "flash_on",
                title: "Fast dev",
                text: "Cras facilisis mi vitae nunc lobortis pharetra. Nulla volutpat tincidunt ornare. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis Nullam in aliquet odio. Aliquam eu est vitae tellus bibendum tincidunt. Suspendisse potenti."
            },
            {
                icon: "build",
                title: "Fast dev",
                text: "Cras facilisis mi vitae nunc lobortis pharetra. Nulla volutpat tincidunt ornare. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis Nullam in aliquet odio. Aliquam eu est vitae tellus bibendum tincidunt. Suspendisse potenti."
            }

        ]

    })
    
}
</script>

<style scoped>

</style>
