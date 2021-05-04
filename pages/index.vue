<template lang="pug">  
.page  
  section-header(  
    title="Nuxt blog"  
    subtitle="My first Nuxt blog ever"  
  )  

  post-list  
</template>  
  
<script lang="ts">  
import Vue from 'vue'  

export default Vue.extend({  
  name: 'HomePage',  
})  
</script>