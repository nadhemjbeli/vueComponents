<template>
  <div id="kings">
    <ul>
      <li v-for="king in kings" v-bind:key="king.id" v-on:click="king.show=!king.show">
        <h1>{{king.name}}</h1>
        <h3 v-show="king.show">{{king.speciality}}</h3>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  components: {},
  data() {
    return {
      kings: [
        { name: "nadhem", speciality: "Vue Components", show: false },
        { name: "latifa", speciality: "HTML Wizardry", show: false },
        { name: "anwer", speciality: "Click Events", show: false },
        { name: "selem", speciality: "Conditionals", show: false },
        { name: "marwen", speciality: "Webpack", show: false },
        { name: "abd rahmen", speciality: "Data Digging", show: false }
      ]
    };
  }
};
</script>

<style scoped>
#kings {
  width: 100%;
  max-width: 1200px;
  margin: 40px auto;
  padding: 0 20px;
  box-sizing: border-box;
}
ul {
  display: flex;
  flex-wrap: wrap;
  list-style-type: none;
  padding: 0;
}
li {
  flex-grow: 1;
  flex-basis: 300px;
  text-align: center;
  padding: 30px;
  border: 1px solid #222;
  margin: 10px;
}
</style>

