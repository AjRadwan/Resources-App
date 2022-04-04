<template>
  <ul>
    <Resources v-for="res in storedResource" 
    :key="res.id"
    :title="res.title"
    :description="res.description"
    :link="res.link" />
  </ul>
</template>

<script>
import Resources from './components/Resources/Resources.vue'

  export default{
  components:{
    Resources
  },

    data(){
      return{
        storedResource:[
          {
            id: "offical guide",
            title: "The offical guide docs",
            description: "the guide to vue js",
            link: "http://vuejs.org",
          },
          {
            id: "goolge guide",
            title: "The goolge guide docs",
            description: "the guide to vue js",
            link: "https://www.youtube.com/",
          }
        ]
      }
    },
    
  }
</script>

<style>
 
</style>
