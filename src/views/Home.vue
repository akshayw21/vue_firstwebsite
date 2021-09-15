<template>
<div>
  <navbar/>
  <crousal/>
  <footer/>
  </div>
</template>

<script>

import crousal from '../components/crousal.vue'
import navbar from '../components/navbar.vue'
import footer from '../components/footer.vue'
  

  export default {
    name: 'Home',
    components: {
        crousal,
        
        navbar,
        footer,
  },
 
  }

  
    
  
</script>
