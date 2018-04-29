<template>
<div class=projects>
    <div class="container">
    <div id="items">
    <v-flex xs10 offset-xs1>
    <div class="card" v-for="card in cards" :key="card">
        <div class="card-content">
            <p class="title">
                {{card.title}}
            </p>
            <p class="subtitle">
                {{card.description}}
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

  <!-- <ol>
    <li v-for="todo in todos" :key="todo">
      {{ todo.text }}
    </li>
  </ol> -->
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
    }
    .card {
        margin: 2em 2em;
    }

    #items {
        /* padding: 4em 15em 4em 15em; */
        /* padding-top: 4em;
        padding-left: 15em;
        padding-right: 15em; */
        padding: 0.25em;
        background-color:rgb(86, 97, 100);
    }

</style>
<script>

  export default {
    data: () => ({
      cards: [
        {title: 'Reverse Polish Notation Calculator', link: '/static/github.png', description:'Reverse Polish Notation (RPN) provides the quickest way to enter data in a calculator because it eliminates the need for parenthesis. It is a way of writing a mathematical expressions where each operand is preceded by the two operators it applies to'},
        {title: 'Inpainting', link: '/static/github.png', description:'Inpainting is the process of reconstructing lost or deteriorated parts of images and videos. In the museum world, in the case of a valuable painting, this task would be carried out by a skilled art conservator or art restorer. In the digital world, inpainting (also known as image interpolation or video interpolation) refers to the application of sophisticated algorithms to replace lost or corrupted parts of the image data (mainly small regions or to remove small defects).'},
        {title: 'Burger Queen', link: '/static/github.png', description:'the purpose of this project is to let you order your fast food through an app using MVC architecture thanks to JavaFX'}
      ],
    //   todos: [
    //   { text: 'Learn JavaScript' },
    //   { text: 'Learn Vue' },
    //   { text: 'Build something awesome' }
    // ]
    })
    
  }
  
</script>


