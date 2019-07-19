<template>

  <div>
    <button v-on:click="decrease"> - </button>
    <span> {{ count }} </span>
    <button v-on:click="increase"> + </button>
  </div>

</template>

<script>

export default {
  name: 'app',
  data() {
    return {
      count: 0
    }
  },
  methods: {
    increase() {
      this.count ++;
    },
    decrease() {
      this.count --;
    }
  }

}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
button{
  margin: 30px;
  font-size: 30px;
}
span{
  margin: 30px;
  font-size: 30px;
}
</style>
