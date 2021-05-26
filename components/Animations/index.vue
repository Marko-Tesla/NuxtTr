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
    div.flexParent

        witch.six
        
        witch.seven

        witch.eight
        
        witch.nine

        witch.ten
    div.flexParent

        witch.six
        
        witch.seven

        witch.eight
        
        witch.nine

        witch.ten
    div.flexParent

        witch.six
        
        witch.seven

        witch.eight
        
        witch.nine

        witch.ten
    div.flexParent

        witch.six
        
        witch.seven

        witch.eight
        
        witch.nine

        witch.ten
    div.flexParent

        witch.six
        
        witch.seven

        witch.eight
        
        witch.nine

        witch.ten
    
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

.six{
    grid-area: 1/4;
}

.seven{
    grid-area: 2/3;
}

.eight{
    grid-area: 3/2;
}

.nine{
    grid-area: 4/1;
}

.ten{
    grid-area: 5/2;
}
</style>