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
</style>