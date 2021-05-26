<template lang="pug">  
.page  
    section-header(  
        title="Animations"  
    )

    div.flexParent

        witch.one
        
        witch.two

        witch.three
        
        witch.four

        witch.five
</template>  
  
<script lang="ts">  
import Vue from 'vue'
import Witch from "@/components/Witch/index.vue"; 
import Covers from "@/components/Covers/index.vue"; 
import Intelligent from "@/components/Intelligent/index.vue"; 


export default Vue.extend({  
  name: 'HomePage',
  components: {
    Witch,
    Covers,
    Intelligent
  }
})  

</script>

<style scoped>
.flexParent {
    display: grid;
    grid-template-columns: repeat(5, 20%);
    grid-template-rows: repeat(5, 20%);
    max-width: 1128px;
    min-height: 1000px;
    margin: auto;
	margin-top: 50px;
}
.one{
    grid-area: 1/1;
}

.two{
    grid-area: 2/2;
}

.three{
    grid-area: 3/3;
}

.four{
    grid-area: 4/4;
}

.five{
    grid-area: 5/5;
}
</style>