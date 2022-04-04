<template>
   
    <TheHeader title="RememberMe" />
    <StoredResource :resources="storedResource"/>
   
</template>

<script>
import StoredResource from './components/Resources/StoredResource.vue'
import TheHeader from './components/layouts/TheHeader.vue'
  export default{
  components:{
    StoredResource,
    TheHeader
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
 @import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap');

* {
  box-sizing: border-box;
}

html {
  font-family: 'Roboto', sans-serif;
}

body {
  margin: 0;
}
</style>
