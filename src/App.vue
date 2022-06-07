<template>
  
  <displayNavbar/>;
  <displaycontainer1/>;
  <displayTheContainer2/>;

</template>

<script>
import displayNavbar from './components/Navbar.vue'; 
import displaycontainer1 from './components/Container1.vue';
import displayTheContainer2 from './components/Container2.vue';

export default {
  name: 'App',
  components: {
    displayNavbar,
    displaycontainer1,
    displayTheContainer2
  },
  methods: {
    
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
}

.salut{
  height: 20vh;
  background-color: red;
  font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
  font-size: 2rem;
}
</style>
