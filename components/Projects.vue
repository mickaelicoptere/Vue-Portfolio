<template>
<div class=projects>
    <v-flex xs12>
    <div class="card" v-for="card in cards" :key="card">
        <div class="card-content">
            <h1 class="title">
                {{card.title}}
            </h1>
            <p class=".display-3">
                {{card.description}}
            </p>
        </div>
        <footer class="card-footer">
            <p class="card-footer-item">
                <span>
                    View on <a :href=card.link target="_blank">GitHub !</a>
                </span>
            </p>
        </footer>
    </div>
    </v-flex>
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

 <!-- <v-container grid-list-xl>
    <v-layout v-bind="binding">
      <v-flex>
        <v-card dark color="primary">
          <v-card-text>one</v-card-text>
        </v-card>
      </v-flex>
      <v-flex>
        <v-card dark color="secondary">
          <v-card-text>two</v-card-text>
        </v-card>
      </v-flex>
      <v-flex>
        <v-card dark color="accent">
          <v-card-text>three</v-card-text>
        </v-card>
      </v-flex>
    </v-layout>
  </v-container> -->

</div>

</template>

<style>
#issaCard {
  padding-top: 2em;
  /* width: 50em;
  height: 2em; */
  display: flex;
  align-items: center;
  text-align: center;
}

.media {
  size: 2em;
}
.card {
  margin-top: 2em;
}
</style>
<script>
export default {
  data: () => ({
    cards: [
      {
        title: "Reverse Polish Notation Calculator",
        link:
          "https://github.com/mickaelicoptere/Reverse-Polish-Notation-Calculator",
        description:
          "Reverse Polish Notation (RPN) provides the quickest way to enter data in a calculator because it eliminates the need for parenthesis. It is a way of writing a mathematical expressions where each operand is preceded by the two operators it applies to"
      },
      {
        title: "Inpainting",
        link: "https://github.com/mickaelicoptere/Inpainting",
        description:
          "Inpainting is the process of reconstructing lost or deteriorated parts of images and videos. In the museum world, in the case of a valuable painting, this task would be carried out by a skilled art conservator or art restorer. In the digital world, inpainting (also known as image interpolation or video interpolation) refers to the application of sophisticated algorithms to replace lost or corrupted parts of the image data (mainly small regions or to remove small defects)."
      },
      {
        title: "Burger Queen",
        link: "https://github.com/mickaelicoptere/Burger_Queen",
        description:
          "the purpose of this project is to let you order your fast food through an app using MVC architecture thanks to JavaFX"
      }
    ]
  })
};
</script>


