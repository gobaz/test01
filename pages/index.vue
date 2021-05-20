<template>
  <div class="container">
    <div>
      <navbar/>

      <h1 class="title">
        nuxt03
      </h1>
      <logo/>
      <div class="links">
        <a href="https://nuxtjs.org/" target="_blank" rel="noopener noreferrer" class="button--green">
          Documentation
        </a>
        <a href="https://github.com/nuxt/nuxt.js" target="_blank" rel="noopener noreferrer" class="button--grey">
          GitHub
        </a>
      </div>

      <b-container>
        <div class="bg-light p-5 rounded">
          <h1>Navbar example</h1>
          <p class="lead">This example is a quick exercise to illustrate how fixed to top navbar works. As you scroll,
            it will remain fixed to the top of your browser’s viewport.</p>
          <a class="btn btn-lg btn-primary" href="/" role="button">View navbar docs &raquo;</a>
        </div>
      </b-container>


    </div>
  </div>

</template>

<script>
import main from "@/layouts/main";
import Navbar from "@/components/Navbar";

export default {
  components: {Navbar},
  layout: 'main'
}
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'Quicksand',
  'Source Sans Pro',
  -apple-system,
  BlinkMacSystemFont,
  'Segoe UI',
  Roboto,
  'Helvetica Neue',
  Arial,
  sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

/* Show it is fixed to the top */
body {
  min-height: 75rem;
  padding-top: 4.5rem;
}

.bd-placeholder-img {
  font-size: 1.125rem;
  text-anchor: middle;
  -webkit-user-select: none;
  -moz-user-select: none;
  user-select: none;
}

@media (min-width: 768px) {
  .bd-placeholder-img-lg {
    font-size: 3.5rem;
  }
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
