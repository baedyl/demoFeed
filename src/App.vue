<script setup>
import { RouterView } from "vue-router";
import NavBar from "@/components/NavBar.vue";
</script>

<template>
  <header>
    <div class="wrapper">
      <NavBar />
    </div>
  </header>

  <RouterView />
</template>

<style>
@import "@/assets/base.css";
/* Custom fonts */
@font-face {
  font-family: "Graphik";
  src: local("Graphik"),
    url(./fonts/Graphik/GraphikRegular.otf) format("truetype");
}
@font-face {
  font-family: "GraphikBlack";
  src: local("Graphik"),
    url(./fonts/Graphik/GraphikBlack.otf) format("truetype");
}

#app {
  max-width: 100%;
  padding: 2rem;
  font-weight: normal;
  font-family: "GraphikBlack";
}
hr {
  border: 0;
  height: 1px;
  background-image: linear-gradient(
    to right,
    rgba(136, 136, 136, 0),
    rgba(255, 255, 255, 0.75),
    rgba(138, 136, 136, 0)
  );
  margin-top: 42px;
}
</style>
