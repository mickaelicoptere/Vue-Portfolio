<template>
  <section class="section is-large">
    <div class="container has-text-centered">
      <!-- <transition v-on:enter="enter" -->
        <h1 id="title">Hi, I'm Mickael Lanier</h1>
      <h2 class="subtitle">I'm a <p id="bold">{{whoami}}</p> {{whatido}}</h2>
    </div>
  </section>
</template>

<script>
export default {
  data: () => ({
    whoami: "co-op student",
    whatido:
      "at UNSA institute of technology and i work for the Rector of Nice academy as an IT tech."
  })
};
</script>

<style>
#title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont,
    "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif; /* 1 */
  color: #35495e;
  letter-spacing: 1px;
  align-items: center;
  text-align: center;
  font-weight: 300;
  font-size: 4em;
}
#bold {
  display: inline;
  font-weight: bold;
}
</style>
