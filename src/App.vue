<template>
  <navBar />
  <LancheComponent />
</template>

<script>
import navBar from "./components/navBar.vue";
import LancheComponent from "./components/LancheComponent.vue";
export default {
  name: "App",
  components: {
    navBar,
    LancheComponent,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #052d55;
  margin-top: 0px;
}
</style>
