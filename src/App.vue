<template>
  <ul>
    <learning-resource
      v-for="res in storedResources" 
      :key="res.id"
      :title="res.title"
      :description="res.description"
      :link="res.link"
    ></learning-resource>
  </ul>
</template>

<script>
import LearningResource from './components/Learning-resources/StudyResource.vue';
  export default {
    components: {
      LearningResource,
    },  
    data () {
      return {
        storedResources: [
          {
            id: 'official-guide', 
            title: 'official Guide', 
            description: 'The official Vue.js documentation.',
            link: 'https://vuejs.org'
          },
          {
            id: 'google', 
            title: 'Google', 
            description: 'View in Google....',
            link: 'https://google.org'
          },
        ]
      }
    }
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