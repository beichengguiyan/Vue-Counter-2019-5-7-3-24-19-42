<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h2>counter</h2>
    <input id="text" v-model.number="num" />
    <div v-for="item in num" :key="item">
      {{item}}
      <p>counter</p>  
      <Counter></Counter>
    </div>
  </div>
</template>

<script>
import Counter from "./Counter";
export default {
  name: "HelloWorld",
  data() {
    return {
      num: 0,
      msg: "Welcome to Your Vue.js App"
    };
  },
  components: {
    Counter
  },
  Methods: {}
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
