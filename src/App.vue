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
      <Aside :items="sections"/>
  </main>

</div>
  
  
</template>

<script>
import Header from './components/Header';
import Navbar from './components/Navbar';
import Article from './components/Article';
import Aside from './components/Aside';

export default {

  name: 'App',
  components:{
    Header,
    Navbar,
    Article,
    Aside,
  },
  data(){
    return {
      sections: ['Section 1', 'Section 2', 'Section 3', 'Section 4', 'Section 5', 'Section 6', 'Section 7', 'Section 8', 'Section 9', 'Section 10', 'Section 11', 'Section 12']
    }
  }
  
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
