<template>
<div class='container'>
  <header>
    <Header />
  </header>
  <nav>
    <Navbar />
  </nav>

</div>
  
  
</template>

<script>
import Header from './components/Header';
import Navbar from './components/Navbar';

export default {

  name: 'App',
  components:{
    Header,
    Navbar,
  },
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  max-width: 992px;
  margin: 0 auto;
}
</style>
