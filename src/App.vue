<template>
  <store-resource :resource="storedResources"></store-resource>
</template>

<script>
import StoreResource from './components/Learning-resources/StoreResource.vue';
  export default {
    components: {
      StoreResource,
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