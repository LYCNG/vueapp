<template>
  <div>
    <Counter />
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
// import TestHello from './components/TestHello.vue'
import Counter from './components/Counter.vue'
export default {
  name:"App",
  components:{
    Counter
  }

}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
