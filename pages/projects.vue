<template>
  <section class="section is-medium">
    <div class="container has-text-centered">
      <h1 class="title">My Projects</h1>
        <p>
            Some of my projects can be found on <a href="https://github.com/mickaelicoptere" target="_blank">GitHub</a>.
        </p>
    <projects></projects>
    </div>
  </section>
</template>
<script>
import Projects from '../components/Projects'

  export default {
    components: {
      Projects
    }
  }
</script>