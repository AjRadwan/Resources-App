<template>
  <ul>
    <Resources v-for="res in resources" 
    :key="res.id"
    :title="res.title"
    :description="res.description"
    :link="res.link" />
  </ul>
</template>

<script>
import Resources from "./Resources.vue"

export default {
    props: ['resources'],

components:{
    Resources
  },
}
 
</script>

<style scoped>
ul {
  list-style: none;
  margin: 0;
  padding: 0;
  margin: auto;
  max-width: 40rem;
}

</style>