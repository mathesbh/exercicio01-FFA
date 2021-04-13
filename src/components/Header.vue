<template>
  
  <nav>
    <a href="#"><Logo /></a>
    <ul>      
      <li>Topic1</li>
      <li>Topic2</li>
      <li>Topic3</li>
      <li>Topic4</li>
    </ul>
  </nav>
</template>

<script>
import Logo from '../components/Logo'

export default {
  name: 'Header',
  components: {
    Logo,
  },

}
</script>

<style scoped>
  nav{
    display: flex;
    justify-content: space-between;   
  }

  ul{
    display: flex;
    margin-right: 2%;
    list-style-type: none;
  }

  li{
    cursor: pointer;
    padding-left: 1rem;
  }
</style>