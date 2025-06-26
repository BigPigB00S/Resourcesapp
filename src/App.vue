<template>
  <ul></ul>
</template>

<script>
  export default {
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