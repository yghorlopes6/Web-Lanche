<template>
  <div class="hello">
    <h1>{{ mensagem }}</h1>
  </div>
</template>

<script>
export default {
  name: "ContactPage",
  props: {
    mensagem: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped></style>
