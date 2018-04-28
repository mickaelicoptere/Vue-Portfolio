<template>
<div class=projects>
    <!-- <div class="card">
        <div class="card-content">
            <p class="title">
                Burger Queen
            </p>
            <p class="subtitle">
            Java
            </p>
        </div>
        <footer class="card-footer">
            <p class="card-footer-item">
                <span>
                    View on <a href="https://twitter.com/codinghorror/status/506010907021828096">Twitter</a>
                </span>
            </p>
            <p class="card-footer-item">
                <span>
                    Share on <a href="#">Facebook</a>
                </span>
            </p>
        </footer>
    </div> -->

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
    }

    .media {
        size: 2em;
    }

</style>
<script>

  export default {
    data: () => ({
      cards: [
        {title: 'Project1', src: '/static/github.png'},
        {title: 'Project2', src: '/static/github.png'},
        {title: 'Project3', src: '/static/github.png'}
      ],
      todos: [
      { text: 'Learn JavaScript' },
      { text: 'Learn Vue' },
      { text: 'Build something awesome' }
    ]
    })
    
  }
  
</script>


