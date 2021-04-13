<template>
  <aside >
    <section v-for="(item, index) in items" :key="index">
      <h5>{{ item }}</h5>
    </section>
  </aside>
</template>

<script>
export default {
  name: 'Aside',
  props: {
    items: String,
  },
}
</script>

<style scoped>
  aside{
    text-align: center;
  }
</style>