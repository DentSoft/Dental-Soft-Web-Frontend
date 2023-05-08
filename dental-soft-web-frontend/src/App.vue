<template>
  <div>
    <HelloWorld msg="Welcome to Your Vue.js App" />
    <VerticalNavBarVue />
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import VerticalNavBarVue from './components/VerticalNavBar.vue';
export default {
  name: 'App',
  components: {
    HelloWorld,
    VerticalNavBarVue
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Karla&display=swap');
@import url('https://fonts.googleapis.com/css?family=Material+Icons');

#app {
  font-family: Karla, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

a:active,
a:link,
a:visited {
  text-decoration: none;
}

a:hover {
  background-color: #E0F7FA;
}
</style>
