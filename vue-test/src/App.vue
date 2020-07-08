<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
    <!-- <HelloWorld /> -->
    
    <SlotTest url="/profile">
    <template v-slot:header>
      <h1>Here might be a page title</h1>
    </template>
    </SlotTest>
    
  </div> 
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import SlotTest from './components/SlotTest.vue'
export default {
  name: 'App',
  components: {
    // HelloWorld,
    SlotTest
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
