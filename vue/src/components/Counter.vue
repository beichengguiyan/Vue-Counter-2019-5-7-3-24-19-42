<template>
  <div class="counter">
    <button class = "click me" @click="add()">+</button>{{count}}
    <button class = "click me" @click="sub()">-</button>
    
  </div>
</template>

<script>
export default {
  name: 'counter',
  data () {
    return {
      count : 0,
      msg: 'Welcome to Your Vue.js App'
    }
  },
  methods : {
    add : function() {
        this.count++;
    },
    sub: function() {
        this.count--;
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
button{
margin-right:20px;
margin-left:20px;

}
</style>
