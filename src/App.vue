<template>
 <h2>Hello</h2>
  <ul v-if="Stored in storedResource">
    <li> {{Stored.id}}</li>
  </ul>
</template>

<script>
  export default{
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
