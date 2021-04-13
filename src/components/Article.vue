<template>
  <section>    
    <article v-for="(item, index) in items" :key="index">
        <Picture :link="item.linkImg" :title="item.titleImg"/>
        <section>
          <h4>{{ item.title }}</h4>
          <p>{{ item.content }}</p>
        </section>
    </article>
  </section>
</template>

<script>
import Picture from './Picture';

export default {
  name: 'Article',
  components: {
    Picture,
  },
  data(){
    return{
      items: [
        {
          id: 1,
          title: 'Approachable',
          content:'Already know HTML, CSS and JavaScript? Read the guide and start building things in no time!',
          titleImg: 'approachable',
          linkImg: 'https://lh3.googleusercontent.com/proxy/RgDefGdCVQi6IB7tVr2zEOz7x08VqcWT19T5zV5L0F76RFOfQtimPMF5t0BY9Dfia7NJBqN5T77xbmgueOpK2ZyVorz3WgGLv-6nmy_RKq5VtdtdnrTpIEiRO_2N8w'
        },
        {
          id: 2,
          title: 'Versatile',
          content:'An incrementally adoptable ecosystem that scales between a library and a full-featured framework.',
          titleImg: 'versatile',
          linkImg: 'https://images.vexels.com/media/users/3/184630/isolated/preview/47fe502ffe26816c23c21de704b084d8-ilustra-ccedil-atilde-o-de-ferramenta-canivete-su-iacute-ccedil-o-by-vexels.png'
        },
        {
          id: 3,
          title: 'Performant',
          content:'20KB min+gzip Runtime Blazing Fast Virtual DOM Minimal Optimization Efforts',
          titleImg: 'performant',
          linkImg: 'https://worldreliefsacramento.org/sites/default/files/icon-documentation.png'
        },
      ]
    }
  }
}
</script>

<style scoped>
article{
  display: flex;
  margin-bottom: 1%;
  background-color: #bccfe4;
}

article section{
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 5%;
}
</style>