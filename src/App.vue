<template>
<div class='container'>
  <header>
    <Header />
  </header>
  <nav>
    <Navbar />
  </nav>
  <main class='wrapper'>
      <Article />
  
    <aside>
      
    </aside>

  </main>

</div>
  
  
</template>

<script>
import Header from './components/Header';
import Navbar from './components/Navbar';
import Article from './components/Article';

export default {

  name: 'App',
  components:{
    Header,
    Navbar,
    Article,
  },
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin: 0 auto;
  max-width: 1000px;
}

.wrapper{
  display: grid;
  grid-template-columns: 70% 30%;
}

</style>
