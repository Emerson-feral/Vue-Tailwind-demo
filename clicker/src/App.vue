<template>
  <div class="flex">
    <NavBar/>
    <Clicker/>
  </div>
</template>

<script>
import Clicker from './components/Clicker.vue'
import NavBar from './components/NavBar.vue'

  export default{
    name:"App",
    components: { 
      Clicker,
      NavBar 
    },
  }
</script>


<style>

</style>
