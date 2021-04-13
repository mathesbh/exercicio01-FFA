<template>
    <picture>
      <img v-bind:src="link" v-bind:alt="title">
    </picture>
</template>

<script>
export default {
  name: 'Picture',
  props: {
    link: String,
    title: String,
  },  
}
</script>

<style scoped>
picture img{
  width: 250px;
  height: 230px;
}

@media (max-width: 740px) {
  picture{
    display: flex;
    align-items: center;
  }
  picture img{
    width: 150px;
    height: 130px;
  }
}
</style>