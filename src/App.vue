<script>
import axios from 'axios';
import HelloWorld from './components/HelloWorld.vue';

export default {

    components: { HelloWorld },

    data() {
      return {
        
      }
    },

    created() {
      axios.get('http://localhost:8000/api/post')
      .then(resonse => {
        console.log(resonse.data);
      })
    }

};

</script>

<template>
  <div>
    <HelloWorld/>
    
  </div>
</template>

<style lang="scss">
  
</style>