<template>
  <footer>
    <p>{{copyright}}</p>
  </footer>
</template>

<script>
export default {
  components: {},
  data() {
    return {
      copyright: "copyright 2020 vue nads"
    };
  }
};
</script>

<style scoped>
footer {
  background: #222;
  padding: 20px;
}
p {
  color: lightgrey;
  text-align: center;
}
</style>
