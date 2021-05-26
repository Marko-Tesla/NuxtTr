<template lang="pug">  
.page  
  section-header(  
    title="Nuxt blog"  
    subtitle="My first Nuxt blog ever"  
  )  
  
  app-options

  post-list

  animations

</template>  
  
<script lang="ts">  
import Vue from 'vue'
import NavBar from "@/components/Navbar/index.vue"; 

import Animations from "@/components/Animations/index.vue"; 

export default Vue.extend({  
  name: 'HomePage',
  components: {
    NavBar,
    Animations
  }
})  

</script>

