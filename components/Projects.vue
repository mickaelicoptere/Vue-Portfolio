<template>
<div class=projects>
    <div class="container">
    <div id="items">
    <div class="columns is-mobile">
    <!-- <div class="column is-three-fifths is-offset-one-quarter"> -->
    <v-flex xs10 offset-xs1>
    <div class="card" v-for="card in cards" :key="card">
        <div class="card-content">
            <p class="title">
                {{card.title}}
            </p>
            <p class="subtitle">
                {{card.title}}
            </p>
        </div>
        <footer class="card-footer">
            <p class="card-footer-item">
                <span>
                    View on <a href="https://twitter.com/codinghorror/status/506010907021828096">GitHub</a>
                </span>
            </p>
        </footer>
    </div>
    </v-flex>
    <!-- </div> -->
    </div>
    </div>
    </div>
    <!-- <div id='issaCard'>
        <v-layout>
            <v-flex xs12 sm6 offset-sm3>
                <div id="vCards">
                <v-card>
                    <v-card-media v-for="card in cards" :key="card.title">
                        <img class='media' src="~/assets/github.png"> 
                    </v-card-media>
                    <v-card-title primary-title>
                    <div>
                        <h3 class="headline mb-0"> {{card.title}}</h3>
                        <div>Located two hours south of Sydney in the <br>Southern Highlands of New South Wales, ...</div>
                    </div>
                    </v-card-title>
                    <v-card-actions>
                        <v-btn flat color="orange">Share</v-btn>
                        <v-btn flat color="orange">Explore</v-btn>
                    </v-card-actions>
                </v-card>
                </div>
            </v-flex>
        </v-layout>
    </div> -->

  <ol>
    <li v-for="todo in todos" :key="todo">
      {{ todo.text }}
    </li>
  </ol>
</div>

</template>

<style>
    #issaCard {
        padding-top: 2em;
        width: 50em;
        height: 2em;
        display: flex;
        align-items: center;
        text-align: center;
    }

    .media {
        size: 2em;
    }swqqQ
    .card {
        margin-top: 2em;
    }

    #items {
        /* padding: 4em 15em 4em 15em; */
        /* padding-top: 4em;
        padding-left: 15em;
        padding-right: 15em; */
        background-color:lightblue;
    }

</style>
<script>

  export default {
    data: () => ({
      cards: [
        {title: 'Project1', link: '/static/github.png', description:''},
        {title: 'Project1', link: '/static/github.png', description:''},
        {title: 'Project1', link: '/static/github.png', description:''}
      ],
      todos: [
      { text: 'Learn JavaScript' },
      { text: 'Learn Vue' },
      { text: 'Build something awesome' }
    ]
    })
    
  }
  
</script>


