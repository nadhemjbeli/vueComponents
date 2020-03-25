<template>
  <header>
    <h1>{{title}}</h1>
  </header>
</template>

<script>
export default {
  components: {},
  data() {
    return {
      title: "nadhem the king"
    };
  }
};
</script>

<style scoped>
header {
  background: lightgrey;
  padding: 20px;
}
h1 {
  color: #222;
  text-align: center;
}
</style>
