<template>
  <base-card>
    <base-button @click="setSelectedTab('stored-resources')">Stored Resources</base-button>
    <base-button @click="setSelectedTab('add-resources')">Add Resources</base-button>
  </base-card>

  <component :is="selectedTab"></component>
</template>

<script>
import StoredResource from './StoredResource.vue'
import AddResources from './AddResources.vue'
 

export default {
    components:{ 
      StoredResource,
      AddResources
    },
 data() {
     return {
         selectedTab: 'stored-resources',
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
provide(){
  return{
      resources: this.StoredResource
  }
},

 methods: {
     setSelectedTab(tab){
          this.selectedTab = tab;
     }
 },
}
</script>

<style>

</style>